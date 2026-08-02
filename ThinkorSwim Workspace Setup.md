# 5MTC Slower Paced Study Group — thinkorswim Workspace Setup

This guide gets your thinkorswim charts matching the group's standard layout: ES / SPX / /NQ three-panel grid, VWAP, 9/21 EMAs, and the custom cross-signal alert.

---

## Step 1: Import the Shared Workspace

1. Open thinkorswim
2. Click **Setup** (top-right corner)
3. Select **Open shared item...**
4. Paste this link into the **Shared item URL** field:

```
   https://tos.mx/!4X8YHzF6
```

5. Click **Preview**, then **Import**

This should bring in the chart grid layout, symbols, timeframes, and built-in studies (VWAP, 9 EMA, 21 EMA, VolumeAvg).

**Note:** custom studies don't always transfer reliably through shared workspace links. After importing, check your **ES chart** on the left-hand-side — if you don't see green/red arrows marking EMA crosses, follow Step 2 below to add it manually.

---

## Step 2: Add the Custom EMA 9/21 Cross Signal Study

1. On any chart, click the **Studies** icon (flask icon, top right)
2. Click **Edit Studies**. A window called **Edit Studies and Strategies** will open.
3. Click **Create** (bottom left of the dialog)
4. Name it exactly: `EMA_9_21_Cross_Signal`
5. Delete any placeholder code in the editor, and paste the following:

```
# 9/21 EMA Cross Signal
declare upper;

input fastLength = 9;
input midLength = 21;
input price = close;

def fastEMA = ExpAverage(price, fastLength);
def midEMA = ExpAverage(price, midLength);

plot BullCross = if fastEMA crosses above midEMA then midEMA else Double.NaN;
BullCross.SetPaintingStrategy(PaintingStrategy.ARROW_UP);
BullCross.SetDefaultColor(Color.GREEN);
BullCross.SetLineWeight(3);

plot BearCross = if fastEMA crosses below midEMA then midEMA else Double.NaN;
BearCross.SetPaintingStrategy(PaintingStrategy.ARROW_DOWN);
BearCross.SetDefaultColor(Color.RED);
BearCross.SetLineWeight(3);

Alert(fastEMA crosses above midEMA, "9/21 EMA Bull Cross", Alert.BAR, Sound.Ding);
Alert(fastEMA crosses below midEMA, "9/21 EMA Bear Cross", Alert.BAR, Sound.Ding);
```

6. Click **OK** to save it
7. Back on your **ES, SPX and SPY charts**, click **Studies** (flask incon) **→ Add Study → Custom** → find `EMA_9_21_Cross_Signal` → add it

---

## Quick Reference: Study Assignments

| Chart | Studies |
|---|---|
| **ES** | VWAP (-2.0 / 2.0, DAY), VolumeAvg (50), EMA_9_21_Cross_Signal |
| **SPX** | EMA (9, close), EMA (21, close), EMA_9_21_Cross_Signal |
| **/NQ** | Optional: same as ES |

> **Why no VWAP on SPX?** SPX is a cash index with no real volume data, so VWAP won't render there. VWAP context comes from the ES chart instead.

---

*Questions? Drop them in the Facebook group  — this is a study group, we're all figuring this out together.*
