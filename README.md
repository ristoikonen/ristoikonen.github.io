

# Projects

- [AWS](https://github.com/ristoikonen/Embed.AppHost/blob/master/FV.md) -  My AWS Lambda finacial functions

- [PixMapper Class Library](https://github.com/ristoikonen/PixMapper) - Encodes text into a Bitmap, reads text from a Bitmap. Unique encoder as edits can be easily verified using image editor. Original idea, code is 100% by me.

- [PDF_Llama](https://github.com/ristoikonen/PDF_Llama) -  Use Ollama models to summarise and analyse PDF's. PDF are read using PDFPig.

Code to find closest color to the eye.

```csh

// How close are two pixels colors.
public double ColourDistance(BGRA e1, BGRA e2)
{
    long rmean = ((long)e1.Red + (long)e2.Red) / 2;
    long r = (long)e1.Red - (long)e2.Red;
    long g = (long)e1.Green - (long)e2.Green;
    long b = (long)e1.Blue - (long)e2.Blue;
    return Math.Sqrt((((512 + rmean) * r * r) >> 8) + 4 * g * g + (((767 - rmean) * b * b) >> 8));
}

```
