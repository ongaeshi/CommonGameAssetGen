# CommonGameAssetGen
Generate game assets according to the [CommonGameAssetRule](https://github.com/ongaeshi/CommonGameAssetRule) using the OpenAI API.

# Install
Use [runa](https://github.com/ongaeshi/runa).

```
$ gem install runa
```

Clone repository.

```
$ git clone https://github.com/ongaeshi/CommonGameAssetGen.git
$ cd CommonGameAssetGen
$ runa install
$ rune deploy cgagen /path/to/bin
```

Create `.token` file.

```
$ echo "WRITE_OPEN_AI_TOKEN" > .token
```


# Usage
Create yaml setting file.

```yaml
thema: "Halloween"

- kind: "player1"
  description: "Cute Ghost"
- kind: "enemy1"
  description: "Scary Pumpkin"
- kind: "weapon1"
  description: "Fireball"
- kind: "item1"
  description: "Lucky Coin"
- kind: "tile1"
  description: "Brick wall"
- kind: "background1"
  description: "Night Pumpkin's dark castle"
```

Execute and generate assets.

```
$ cgagen asset.yml
Save to player1_20231217002720.png
Save to enemy1_20231217002720.png
Save to weapon1_20231217002720.png
Save to item1_20231217002720.png
Save to tile1_20231217002720.png
Save to background1_20231217002720.png
```

