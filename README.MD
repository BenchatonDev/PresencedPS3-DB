# Presenced PS3 Icon DB

A set of json files to map PS3 and PSP TitleIDs to 512x512 icons for [Presenced](https://github.com/BenchatonDev/Presenced).

> [!Attention]
> This is just for legal context but this repo only hosts images and a way to link a game to one of said images. It does NOT claim ANY of it's content under a license, by default and by Github's TOS any repo without a `LICENSE` file is classified as *`All Rights Reserved`*. This notice is here to clarify that it's not the case here since I can't just re-license the work of other as my own under any license other than the original one unless compatible or with authorization from the artist or IP holder

# How to help ?

First things first take a look at the [TitleID](titleids.json) list to see if your game is already referenced by it's international release name (for non region exclusive games). Already there ? There are other ways to help !

> [!Tip]
> A game may be in the [TitleID](titleids.json) file but not have an icon, double check in the [Icons](icons.json) file if you're unsure

### Not there ?

Then I advise you to go look at the [PS3 TitleID Database](http://ps3.aldostools.org/titleid.html) and search for your game's name, then add all titles IDs that refer to the your game to the [TitleID](titleids.json) json file like this:

```json
{
    [...]
    "BLET70052": "Ace Combat Infinity",
    "NPJB90677": "Ace Combat Infinity",
    "NPUB31420": "Ace Combat Infinity",
    "NPEB01839": "Ace Combat Infinity",
    "NPUB31347": "Ace Combat Infinity",
    "NPJB00481": "Ace Combat Infinity",
    [...]
}
```

Once your game's TitleIDs all map to one name you can add your `512x512` icon's jpeg file name to the [Icons](icons.json) json file like this:

```json
{
    [...]
    "Ace Combat Infinity": "AC-Infinity.jpg",
    [...]
}
```

When naming you icon file there are a few things to consider, first it needs to be unique, match / have some relation to the game's name and finally it shouldn't be too long but still readable

### Already there ?

As of now, the addition of new tittles is really manual and tedious, a fancy helper script with good human supervision features would go a long way streamlining the contributing process, sadly I have no idea how to do that but please don't make it 100% using *"AI"* else it would already exist in the repo.

# Acknowledgements
- [Aldostools](https://github.com/aldostools) Providing a nice and easely browsable TitleID database