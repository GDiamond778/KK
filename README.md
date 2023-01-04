# Damage-Calculator

This is the repository for the Kinalite Kingdom Damage Calculator

## Contributing

There are 3 areas you can contribute to: kinalite data, moves data, and set data.

For kinalite data, follow this template: 

```js
    azulon: {
        name: "Azulon",
        number: 1,
        types: ["Wood", "None"],
        baseStats: {
            hp: 34,
            energy: 70,
            attack: 80,
            defense: 45,
            attackR: 27,
            defenseR: 50,
            speed: 44
        }
    }
```

For move data, follow this template: 

```js
    hazer: {
        name: "Hazer",
        power: 40,
        type: "Light",
        mr: "Ranged",
        contact: true,
        hits: 3,
        aoe: true,
        secondaryEffect: true,
        drain: 1/3,
        recoil: 1/4
    }
```
If the move doesn't make contact, is single hit, not aoe, doesn't have a secondary effect, doesn't have a drain effect or a recoil effect, don't include that property at all. The first 4 must be included, last 4 are optional.

For set data, follow this template: 

```js
    {
        name: "Miralo",
        setName: "Mixed Tank",
        evs: {
            hp: 5,
            energy: 0,
            attack: 0,
            defense: 3,
            attackR: 0,
            defenseR: 4,
            speed: 0
        },
        moves: {
            move1: "Hazer",
            move2: "Magic Gem",
            move3: "placeholder",
            move4: "placeholder"
        },
        posNature: "vigilant",
        negNature: "lax",
        ability: "Reflector",
        item: "plceholder",
        level: 50
    }
 ```
 Please be aware that everything is case sensitive so natures must be lowercase, abilities, items, and moves all capitalized. I'd recommend keeping level at level 50. Other than that, make any set you want.
