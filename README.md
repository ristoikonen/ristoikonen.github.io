

# Projects

Codings




- [JKM](https://github.com/ristoikonen/JKM) -  Extract spot prices

- [EkaWebAPI](https://github.com/ristoikonen/EkaWebAPI) -  Music streaming API

Learnings
- [Letslearn-dotnet-aspire](https://github.com/ristoikonen/letslearn-dotnet-aspire) - Two APIs in Aspire dashboard

Just for Fun!

- [Bserver](https://github.com/ristoikonen/bserver) -  From Bitmap to collection of bytes to Bitmap; Use LINQ to edit pixels in a List of bytes in between. Check method GetBitmapFromBuGeRedList


How close are colors of two pixels. Using  BGRA as alpha included (vs RGB)

```csh

// How close are colors of two pixels.
public double ColourDistance(BGRA e1, BGRA e2)
{
    long rmean = ((long)e1.Red + (long)e2.Red) / 2;
    long r = (long)e1.Red - (long)e2.Red;
    long g = (long)e1.Green - (long)e2.Green;
    long b = (long)e1.Blue - (long)e2.Blue;
    return Math.Sqrt((((512 + rmean) * r * r) >> 8) + 4 * g * g + (((767 - rmean) * b * b) >> 8));
}

```
