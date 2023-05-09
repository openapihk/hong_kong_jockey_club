# Hong Kong Jockey Club

## Test
1. Retreive session cookie from https://bet.hkjc.com/marksix/index.aspx?lang=ch
2. Update session cookie to cookie-jar.json
3. Run newman with cookie-jar.json
```bash
newman run --verbose tmp/working/tmpCollection.json --cookie-jar cookie-jar.json
```