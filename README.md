# HF_Dutch2Flemish
Dutch2Flemish is an efficient, lightweight tool that automatically converts Dutch text into natural Flemish variants. It is specifically designed to address subtle yet important linguistic differences between the Netherlands and Flanders, ensuring content is both locally accurate and contextually authentic.

## Dutch2Flemish Workflow

**Step-by-step process for translating HelloFresh recipes from Dutch to Flemish:**

1. **🇬🇧 English Recipe File**  
   - Original content created in English.

   ⬇️

2. **📝 Manual Translation to Dutch**  
   - The Dutch team translates the weekly recipe file from English to Dutch manually.

   ⬇️

3. **🤖 Flemishmaker2_0.ipynb (Python Script)**  
   - Processes the Dutch file using `Flemishreplacementsheet1.xlsx` and built-in script nuances.  
   - Automatically converts Dutch to Flemish while preserving formatting (bullet points, bold, italics, headings).

   ⬇️

4. **📄 Formatting with BoldAndItalicmaker**  
   - Copy the translated text into the `BoldAndItalicmaker` tool.  
   - The function `boldAndItalicizeSpecificWords()` applies:
     - **Bold** to key phrases: `"Tip:"`, `"Weetje:"`, `"Gezondheidstip:"`  
     - **Italic** to special phrases: `"(let op: pikant! Gebruik naar smaak)"` etc.  
     - Cleans bullet points and ensures vertical alignment.

   ⬇️

5. **🚀 Ready-to-upload File**  
   - Final file is formatted and ready to be uploaded into the HelloFresh CPS recipe system.  
   - Saves approximately **two full days of manual work per recipe week** while ensuring consistency and quality.


## How Dutch2Flemish Works

The workflow for translating HelloFresh recipe content from Dutch to Flemish is designed to be efficient, accurate, and format-preserving. Here's how it works:

1. **Manual Translation to Dutch**  
   - The Dutch team first translates the weekly recipe file from English to Dutch manually.

2. **Automated Flemish Conversion**  
   - The translated Dutch file is then processed using the Python script `Flemishmaker2_0.ipynb`.  
   - The user specifies the location of the file to be translated, and the script automatically handles the conversion using:  
     - A replacement sheet: `Flemishreplacementsheet1.xlsx`  
     - Built-in linguistic rules and nuances for proper Flemish adaptation  
   - The tool preserves formatting including bullet points, bold, italics, and headings, ensuring content is ready for HelloFresh systems.

3. **Formatting Enhancements with BoldAndItalicmaker**  
   - After translation, the text is copied into the `BoldAndItalicmaker` tool.  
   - This tool contains the function `boldAndItalicizeSpecificWords()`, which:  
     - Identifies key phrases such as `"Tip:"`, `"Weetje:"`, `"Gezondheidstip:"` and makes them **bold**, while the rest of the text is italicized.  
     - Detects special phrases like `"(let op: pikant! Gebruik naar smaak)"` and applies **italic formatting**.  
     - Cleans bullet points and ensures vertical text alignment.  
   - The output file is ready to be uploaded directly into the HelloFresh CPS recipe system.

4. **Efficiency and Consistency**  
   - This workflow eliminates manual adaptation of Dutch text to Flemish while preserving all formatting nuances.  
   - Saves approximately **two full days of manual work per recipe week**, ensuring consistent and high-quality content delivery.

---

### Tools & Files

- `Flemishmaker2_0.ipynb` – Main Python script for Dutch → Flemish conversion  
- `Flemishreplacementsheet1.xlsx` – Sheet containing Dutch → Flemish replacements and rules  
- `BoldAndItalicmaker` – Google Apps Script tool for formatting bullets, bold, and italics  

