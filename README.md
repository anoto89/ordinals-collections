# Ordinals Collections
#### A place for creators &amp; builders to organize ordinal collections!

## File Structure
```
 .
 ├── ...
 └── collection-name            
     ├── inscriptions.json      
     └── meta.json              
```

## Collection Metadata `meta.json`
```
{
  "name": "",                    # inscription name
  "slug": "",                    # directory name
  "inscription_icon": "",        # collection cover inscription id
  "description": "",             # collection description
  "twitter_link": "",            # official twitter
  "discord_link": "",            # official discord
  "website_link": ""             # official website
}
```

## Inscription Data `inscriptions.json`
```
[
  {
    "id": "",                    # inscription id
    "meta": { 
      "name": ""                 # inscription name
    }
  },
  ...
]
```

## Expanding Inscription Data
Collections can be organized using `status` and `rank`
```
[
  {
    "id": "",
    "meta": {
      "name": "",
      "status": "",               # inscription theme
      "rank":                     # inscription rarity rank
    }
  },
  ...
]
```
Artists can assign unqiue traits to ordinals with `attributes`
```
[
  {
    "id": "",
    "meta": {
      "status": "",
      "rank": ,
      "name": ""
      "attributes": [
        {
          "trait_type": "",        # trait category
          "value": "",             # trait value
          "status": "",            # trait theme
          "percent": ""            # percent of inscriptions in collection with trait
        },
        ...
      ]
    }
  },
  ...
]
```

