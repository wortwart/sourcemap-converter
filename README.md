# sourcemap-converter
** Reads and analyzes Base64 VLQ coded source mappings **

* This project was created for an article in [c't Magazin](https://ct.de/). *

JavaScript and basic styling are included in the HTML. Just enter Base64 VLQ code from any sourcemap. The converter will discard anything which is not Base64 - `[A-Za-z0-9+/]` - , comma, or semicolon. Typically, mappings look lik that:

    aAAA,GAAM,OAAQ,QAAR,MAAQ,aAAQ,SAAQ,GAAR,CAAY,UAAY,IAAxB,CAAR,CAAd
    
Or like that:

    AAIA,E,CAJA,C,CACC,eAQA,yB,CALD,E,CACC,kBASA,O,CAKD,I,CAIC,cACA,eACA,W
    
Or like that:

    CAAC,WACA,IAAK,IAAIA,EAAU,EAAGA,EAAU,EAAGA,IAClCC,QAAQC,IAAIF
    
sourcemap-converter tries to make sense of that, according to [Sourcemaps spec v3](https://docs.google.com/document/d/1U1RGAehQwRypUTovF1KRlpiOFze0b-_2gc6fAH0KY0k/edit).
