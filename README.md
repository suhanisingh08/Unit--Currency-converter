# Unit and Currency Converter

**Student:** Suhani | 2nd Year CSE-IOT III Sem | USN: 25BTRCO051

A converter for length, weight, temperature and live currency exchange rates.

## OVERVIEW
The converter has four tabs. The user enters an amount, picks the From and To units, and sees the result instantly. A Swap button reverses the pair.

## TECH STACK
- Frontend: HTML5, CSS3 (Grid, Flexbox, focus styles)
- Logic: vanilla JavaScript (objects of conversion factors, async/await, fetch, Intl number formatting)
- Data: Frankfurter exchange-rate API (free, no key)
- Storage: browser localStorage for the last downloaded rates

## HOW IT WORKS
Length and weight units are stored as factors relative to one base unit, so a conversion is value x from-factor / to-factor. Temperature uses formulas that go through Celsius. For currency, the app downloads rates against USD once, then converts as value / rate(from) x rate(to). The rates are saved, so if the internet is down later, the app uses the last saved rates and says so. Results are formatted with up to six decimals.

## KEY FEATURES
- Length, weight, temperature and currency tabs
- Instant conversion as you type
- Swap button
- Live exchange rates with an offline fallback
- Rate date shown under the result

## USES
Everyday conversions, and practice with data-driven code, API calls and number formatting.

## HOW TO RUN
Open index.html in a browser. Length, weight and temperature work offline; the currency tab needs internet the first time.
