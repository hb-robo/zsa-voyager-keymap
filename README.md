# zsa-voyager-keymap

This is my keymap for my daily-driver keyboard, the ZSA Voyager. You can explore the keymap in your browser on Oryx here: https://configure.zsa.io/voyager/layouts/NXVP6/latest/0

## housekeeping

I'm able to mirror my layout changes from ZSA's Oryx keymap editor (which has proprietary source control) to this repo through the efforts of Pierre Poulain ([@poulainpi](https://github.com/poulainpi)). You can do this yourself by following [this blog, highlighted by ZSA themselves](https://blog.zsa.io/oryx-custom-qmk-features).

## background

The Voyager is a split, columnar, wired 52-key keyboard that looks like this:

![a picture of my white ZSA Voyager split keyboard. It has a 52-key layout, with 4 rows of 6 keys and two thumb buttons per side. The top row keys is totally unused/deactivated for ergonomic reasons](https://github.com/user-attachments/assets/9900abc4-bc69-485e-a865-5d9fba9cd13e)


I've had this keyboard since February 2025. This came about when I started putting consistent effort into practicing touch typing for the first time. I found the assymetry of my no-name chiclet keyboard to cause significant pain as my typing speed increased. It dawned on me that I likely adopted suboptimal typing habits *specifially to avoid this kind of hand discomfort*. Next thing I knew, I was down the ergomech rabbit hole.

There are a number of quality split keyboard options out there, but I landed on the Voyager for a few reasons:
1. It needed to travel well between the office and home so I could practice
2. I saw a number of comments mentioning larger/more complex thumb clusters cause thumb ligament strain
3. I wasn't interested in building it myself or risking a cheaper option with worse QC
4. Access to ZSA Oryx, probably the best keymap software in the business, especially for beginners
5. It uses low-profile Choc switches, which have a shorter travel and wider keycaps than the usual MX variety
6. They offered "blank" keycaps (desirable for touch typing practice) that still allowed for RGB hinting

# keymap walkthrough and justifications

TBD...

## current pain points

Each time an iteration of this keymap fixes something I previously found annoying, my attention is drawn to the next-most annoying thing. Here are some of the problems I'm running into:

1. **The gaming layer doesn't feel good, especially with existing muscle memory.**
    * For ergonomic parity with normal keyboard use, it makes sense to shift WASD under ESDF. This both reduces access to "natural" feeling access to TGBYHN -  commonly used for social functions, grenade throws, thanking the bus driver, etc. - and will cause muscle-memory confusion with screen prompts.
    * **NOTE**: this is easily solved by creating custom key binds in-game to correct key prompts, but I am unwilling to do that for every game. It is also more fragile than changing the keymap itself, requiring in-game remappings every time the keymap is updated.
       * This is also easily solved by a dedicated gaming keyboard (or one-hand-claw-thing), which I am considering.
2. **The thumb clusters don't switch layers fast enough**
    * I'd like to enable "flow tap" on these keys only, which isn't yet supported in Oryx but is in the QMK spec. This would mean that the hold action (kicking off various layers) would execute as soon as another button is pressed.
    * I purposely designed the thumb clusters to be key-combo terminators, so we can safely assume any held-ish action starting with them is to access a key on a layer.
    * This would mean a fast "Space, J" would correctly resolve to ")": the character accessed with the J key while the space hold layer is activated. I just need to tune it so that normal sentence typing isn't affected.
