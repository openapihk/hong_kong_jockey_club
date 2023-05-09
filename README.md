# Hong Kong Jockey Club

## Test
1. Generate collection
```bash
portman -l marksix.yaml -t
```
2. Retreive session cookie from https://bet.hkjc.com/marksix/index.aspx?lang=ch
3. Update session cookie to cookie-jar.json
4. Run newman with cookie-jar.json
```bash
newman run --verbose tmp/working/tmpCollection.json --cookie-jar cookie-jar.json
```