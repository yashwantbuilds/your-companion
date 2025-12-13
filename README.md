# Utility Tools Website

A clean, simple web application with multiple useful tools. Currently includes JSON Beautifier, Regex Find & Replace, Cron Expression Builder, Timezone Converter, Date Calculator, and Text Case Converter.

## Features

### 📄 JSON Beautifier
- **Beautify JSON** - Format JSON with custom indentation
- **Minify JSON** - Compress JSON into a single line
- **Validate JSON** - Check JSON syntax with error messages
- **Copy & Download** - Export your work easily
- **Upload** - Load JSON files directly

### 🔍 Regex Find & Replace
- **Find All** - Search text using regex patterns
- **Replace All** - Replace matches with custom text
- **Regex Flags** - Global, case-insensitive, multiline modes
- **Capture Groups** - Use $1, $2 for group references
- **Common Examples** - Built-in pattern templates

### ⏰ Cron Expression Builder
- **Generate Expressions** - Build cron by filling fields
- **Parse Expressions** - Convert to human-readable descriptions
- **10 Presets** - Quick templates for common schedules
- **Full Validation** - Instant syntax feedback
- **Complete Reference** - Learn cron format and operators

### 🌍 Timezone Converter
- **Multi-timezone Support** - 15 major world timezones
- **Real-time Conversion** - Convert times instantly
- **Easy Selection** - Simple dropdown interface
- **Copy Results** - Export conversions
- **No External API** - All processing local

### 📅 Date Calculator
- **Days Between Dates** - Calculate exact days between two dates
- **Multiple Units** - Get result in weeks, months, years, and hours
- **Instant Calculation** - Real-time computation
- **Copy & Download** - Export your results
- **Accurate Calculations** - Accounts for leap years

### 🔤 Text Case Converter
- **10 Conversion Types**:
  - UPPERCASE
  - lowercase
  - Capitalize
  - Title Case
  - Sentence case
  - tOGGLE cASE
  - esreveR (reverse)
  - camelCase
  - kebab-case
  - snake_case
- **Live Preview** - See changes instantly
- **Character & Word Count** - Track text metrics
- **Copy & Download** - Export converted text

## Getting Started

### Quick Start
1. Open `index.html` in your web browser
2. Use the sidebar to navigate between utilities
3. Try out different features

### File Structure
```
util-ads/
├── index.html    (Complete standalone web application with 6 utilities)
└── README.md     (This file)
```

## How to Use Each Utility

### JSON Beautifier

1. **Beautify JSON**
   - Paste JSON in the input field
   - Click "✨ Beautify" button
   - Formatted JSON appears in the output field

2. **Minify JSON**
   - Enter JSON in the input field
   - Click "📦 Minify" button
   - Get compact single-line JSON

3. **Upload a File**
   - Click "📁 Upload" button
   - Select a `.json` or `.txt` file
   - JSON is loaded into the input field

4. **Change Indentation**
   - Use the "Indent:" dropdown
   - Re-beautify to apply new indentation

### Regex Find & Replace

1. **Find Text**
   - Paste text in the input field
   - Enter a regex pattern (e.g., `\d+` for numbers)
   - Click "🔍 Find All"
   - All matches appear in the output field

2. **Replace Text**
   - Enter text in the input field
   - Enter regex pattern
   - Enter replacement text
   - Click "🔄 Replace All"
   - Modified text appears in output

3. **Regex Flags**
   - **Global**: Find all occurrences (default: checked)
   - **Case insensitive**: Ignore case in matching
   - **Multiline**: Treat ^ and $ as line boundaries

4. **Capture Groups**
   - Use parentheses in pattern: `(\d+)-(\w+)`
   - Reference in replacement: `$2_$1` to swap groups

## Cron Expression Builder

### How to Use

1. **Generate Expression**
   - Fill in the fields (minute, hour, day, month, weekday)
   - Click "🔨 Generate Expression"
   - Expression appears with human-readable description

2. **Parse Expression**
   - Paste a cron expression in the textarea
   - Click "📖 Parse Expression"
   - Get a human-readable description

3. **Use Presets**
   - Click any preset button to load a common schedule
   - Expression and description update instantly

4. **Copy & Download**
   - Click "📋 Copy" to copy to clipboard
   - Click "⬇️ Download" to save as text file

### Cron Format

```
Field 1: Minute        (0-59)
Field 2: Hour          (0-23)
Field 3: Day of Month  (1-31)
Field 4: Month         (1-12 or JAN-DEC)
Field 5: Day of Week   (0-6 or SUN-SAT, 0=Sunday)
```

### Operators

| Operator | Meaning | Example |
|----------|---------|---------|
| `*` | Any value | `*` = every value |
| `,` | List | `1,3,5` = 1, 3, or 5 |
| `-` | Range | `1-5` = 1 through 5 |
| `/` | Step | `*/5` = every 5 |
| `?` | No specific value | Used in day/weekday |

### Common Cron Examples

| Expression | Meaning |
|------------|---------|
| `0 * * * *` | Every hour at minute 0 |
| `0 0 * * *` | Daily at midnight |
| `0 9 * * 1-5` | Weekdays at 9 AM |
| `0 0 * * 0` | Every Sunday at midnight |
| `0 0 1 * *` | First day of month at midnight |
| `*/5 * * * *` | Every 5 minutes |
| `0 */6 * * *` | Every 6 hours |
| `0 12 * * *` | Daily at noon |
| `0 0 15 * *` | 15th of month at midnight |
| `*/15 * * * *` | Every 15 minutes |

### Timezone Converter

1. **Select Date & Time**
   - Choose a date and time using the datetime picker
   - Or type directly: YYYY-MM-DDTHH:MM

2. **Choose Timezones**
   - Select source timezone from dropdown
   - Select target timezone from dropdown
   - Click "🔄 Convert"

3. **View Results**
   - Source time displays with selected timezone
   - Target time shows the converted time
   - Click "📋 Copy" to copy both times

**Supported Timezones:**
- UTC
- America/New_York (Eastern)
- America/Chicago (Central)
- America/Denver (Mountain)
- America/Los_Angeles (Pacific)
- Europe/London
- Europe/Paris
- Europe/Berlin
- Asia/Tokyo
- Asia/Shanghai
- Asia/Hong_Kong
- Asia/Singapore
- Asia/Dubai
- Asia/Kolkata (India)
- Australia/Sydney
- Australia/Melbourne

### Date Calculator

1. **Select Two Dates**
   - Click Date 1 field and select a date
   - Click Date 2 field and select another date
   - Click "📊 Calculate"

2. **View Results**
   - Days between the dates (prominently displayed)
   - Weeks between
   - Months (approximate)
   - Years (approximate)
   - Hours between

3. **Copy Results**
   - Click "📋 Copy" to copy all calculations
   - Results formatted for easy pasting

**Example:**
- Date 1: 2025-01-01
- Date 2: 2025-12-31
- Result: 364 days, 52 weeks, 11 months, 0 years

### Text Case Converter

1. **Paste or Type Text**
   - Enter text in the input field
   - Live character and word count appears

2. **Choose Conversion**
   - Click any case conversion button
   - Result appears in preview area

3. **Available Conversions**
   - **UPPERCASE** - All letters capitalized
   - **lowercase** - All letters lowercased
   - **Capitalize** - First letter uppercase, rest lowercase
   - **Title Case** - Each word starts with capital
   - **Sentence case** - First letter capital, rest lowercase
   - **tOGGLE cASE** - Flip every character's case
   - **esreveR** - Reverse the entire text
   - **camelCase** - Joined words with caps (no spaces/dashes)
   - **kebab-case** - Words joined with hyphens, lowercase
   - **snake_case** - Words joined with underscores, lowercase

4. **Export**
   - Click "📋 Copy" to copy result
   - Click "⬇️ Download" to save as .txt file

**Examples:**
- Input: `hello world` 
  - UPPERCASE → `HELLO WORLD`
  - Title Case → `Hello World`
  - camelCase → `helloWorld`
  - snake_case → `hello_world`
  - kebab-case → `hello-world`

## Common Regex Patterns

| Pattern | Usage | Example |
|---------|-------|---------|
| `\d+` | Numbers | `123`, `456` |
| `\w+` | Words | `hello`, `world123` |
| `\s` | Whitespace | Spaces, tabs, newlines |
| `.` | Any character | Matches anything |
| `*` | 0 or more | `a*b` matches `b`, `ab`, `aab` |
| `+` | 1 or more | `a+b` matches `ab`, `aab` |
| `?` | 0 or 1 | `colou?r` matches `color`, `colour` |
| `^` | Start of line | `^Hello` |
| `$` | End of line | `world$` |
| `[\w.-]+@[\w.-]+\.\w+` | Email | `user@example.com` |

## Examples

### JSON Example
Input:
```json
{"name":"John","age":30,"city":"New York","hobbies":["reading","gaming"]}
```

Output (after beautify):
```json
{
    "name": "John",
    "age": 30,
    "city": "New York",
    "hobbies": [
        "reading",
        "gaming"
    ]
}
```

### Regex Find Example
- **Text**: `Hello 123 World 456 Test 789`
- **Pattern**: `\d+`
- **Result**: `123`, `456`, `789`

### Regex Replace Example
- **Text**: `Name: John Age: 30`
- **Pattern**: `([A-Za-z]+): ([A-Za-z0-9]+)`
- **Replacement**: `$2 ($1)`
- **Result**: `John (Name) 30 (Age)`

## Technical Details

- **No Framework** - Pure HTML, CSS, and JavaScript
- **No Dependencies** - Works offline, no external libraries needed
- **Browser Support** - Works on all modern browsers (Chrome, Firefox, Safari, Edge)
- **Mobile Friendly** - Responsive layout adapts to screen size
- **Local Processing** - All data is processed in your browser, nothing is sent to servers

## Tips

1. **JSON Large Files** - Use Upload for files over 1000 lines
2. **Regex Testing** - Use the examples as templates
3. **Capture Groups** - Use parentheses to group and reuse parts in replacements
4. **Multiline Text** - Enable multiline mode for ^ and $ to work on each line
5. **Escaping** - Use `\\` to escape special characters in regex

## Browser Compatibility

Works on:
- ✅ Chrome/Chromium
- ✅ Firefox
- ✅ Safari
- ✅ Edge
- ✅ Opera
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

## License

Free to use and modify.

## What's Inside

- **Sidebar Navigation** - Easy switching between 6 utilities
- **Responsive Design** - Works on desktop, tablet, and mobile
- **Real-time Processing** - Instant results as you work
- **Professional UI** - Clean, modern interface with gradient backgrounds
- **No Dependencies** - Pure HTML, CSS, and JavaScript
- **Local Processing** - Everything happens in your browser
- **Export Options** - Copy to clipboard or download results
- **Comprehensive Guides** - Built-in references and examples

## Browser Compatibility

Works on:
- ✅ Chrome/Chromium
- ✅ Firefox
- ✅ Safari
- ✅ Edge
- ✅ Opera
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

## Tips & Tricks

### JSON Beautifier
- Auto-beautifies when you paste JSON
- Validate JSON before minifying
- Use different indentation for different APIs

### Regex Find & Replace
- Test patterns on sample text first
- Use capture groups to rearrange text
- Enable multiline for multi-line content

### Cron Expression
- Use presets as templates
- Check your expression with the parser
- Use 1-5 for weekdays (Mon-Fri)

### Timezone Converter
- Note that DST may affect results
- Use UTC as reference timezone
- Copy results for documentation

### Date Calculator
- Calculates inclusive of both dates
- Approximate for months (uses 30.44 days)
- Accurate for leap years

### Text Case Converter
- camelCase and snake_case ignore special characters
- Reverse works on all characters including punctuation
- Word count excludes punctuation-only entries

## License

Free to use and modify.

## Questions?

This is a simple, self-contained application with no external dependencies. Just open it in any modern browser and start using all 6 utilities!
