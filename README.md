# Brüggerei LED Editor

Der Brüggerei LED Editor ist eine Web-App, mit welcher der abzuspielende Inhalt der Brüggerei-LED-Matrix definiert werden kann.

Die Web-App stellt neben einem GUI auch eine http json API bereit, über die der LED-Controller den anzuzeigenden Inhalt abrufen kann.

## API-Schema

```json
{
  "sessions": [
    {
      "text": {
        "startIndex": 2,
        "content": "Hallo",
        "color": [0, 255, 0]
      },
      "lines": [
        {
          "startIndex": 0,
          "color": [255, 255, 0]
        },
        {
          "startIndex": 11,
          "color": [255, 0, 0]
        }
      ],
      "delay": 100
    },
    {
      "text": {
        "startIndex": 2,
        "content": "Mensch",
        "color": [0, 255, 0]
      },
      "lines": [
        {
          "startIndex": 0,
          "color": [255, 255, 0]
        },
        {
          "startIndex": 11,
          "color": [255, 0, 0]
        }
      ],
      "delay": 200
    },
    {
      "text": {
        "startIndex": 2,
        "content": "wie geht es dir?",
        "color": [0, 255, 0]
      },
      "lines": [
        {
          "startIndex": 0,
          "color": [255, 255, 0]
        },
        {
          "startIndex": 11,
          "color": [255, 0, 0]
        }
      ],
      "delay": 100
    }
  ],
  "checksum": "d8fe0511252873a219495e43f72a1d91dbeb2cd939c08dd0c76b2b6cc69cb790"
}
```
