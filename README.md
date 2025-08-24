# zsa-voyager-keymap

This is my keymap for my daily-driver keyboard, the ZSA Voyager. You can explore the keymap in your browser on Oryx here: https://configure.zsa.io/voyager/layouts/NXVP6/latest/0

## housekeeping

I'm able to mirror my layout changes from ZSA's Oryx keymap editor (which has proprietary source control) to this repo through the efforts of Pierre Poulain (@poulainpi). You can do this yourself by following [this blog, highlighted by ZSA themselves](https://blog.zsa.io/oryx-custom-qmk-features).

## background

The Voyager is a split, columnar, wired 52-key keyboard that looks like this:

![a picture of my white ZSA Voyager split keyboard. It has a 52-key layout, with 4 rows of 6 keys and two thumb buttons per side](https://imgur.com/a/WMCE6Px)

I've had this keyboard since February 2025. This came about when I started putting consistent effort into practicing touch typing for the first time. I found the assymetry of my no-name chiclet keyboard to cause significant pain as my typing speed increased. It dawned on me that I likely adopted suboptimal typing habits *specifially to avoid this kind of hand discomfort*. Next thing I knew, I was down the ergomech rabbit hole.

There are a number of quality split keyboard options out there, but I landed on the Voyager for a few reasons:
1. It needed to travel well between the office and home so I could practice
2. I saw a number of comments mentioning larger/more complex thumb clusters cause thumb ligament strain
3. I wasn't interested in building it myself or risking a cheaper option with worse QC
4. Access to ZSA Oryx, probably the best keymap software in the business, especially for beginners
5. It uses Choc switches, which are lower-profile and have wider keycaps than the usual MX variety on mechanical keyboards, reducing potentially straining wrist dorsiflexion
6. They offered "blank" keycaps that still allowed for RGB guiding 

# keymap walkthrough and justifications

TBD...

## current pain points

Each time an iteration of this keymap fixes something I previously found annoying, my attention is drawn to the next-most annoying thing. Here are some of the problems I run into:

1. **The gaming layer doesn't feel good, especially with existing muscle memory.**
    * For ergonomic parity with normal keyboard use, it makes sense to shift WASD under ESDF. This both reduces access to "natural" feeling access to TGBYHN -  commonly used for social functions, grenade throws, thanking the bus driver, etc. - and will cause muscle-memory confusion with screen prompts.
    * **NOTE**: this is easily solved by creating custom key binds in-game to correct key prompts, but I am unwilling to do that for every game. It is also more fragile than changing the keymap itself, requiring in-game remappings every time the keymap is updated.
2. **ESC is not a first-class citizen**.
    * This will probably cost you hours of your life in the long run waiting those 250ms out holding Tab down.
    * I've tried a few changes out in some keymap forks, but nothing feels right yet.
3. **Homerow mods need some tuning.** (to my typing mechanics)
    * Pressing "A, L" too fast triggers a Super+L press, so most times I type "all", it locks my computer on Windows. This is probably due to my left pinky disengaging with the A key too slowly for the mod window to elapse.
    * Simultaneously, "F, -" seems to mostly result in "f-" and not "_". Again, this involves pinky speed, just in the opposite way as before.
4. **Calculators and similar applications don't register the numpad operator keys**
    * The +*-/ keys on the NUM layer are hooked up to a specific variant of those symbols with the "numpad" tag on Oryx. They don't seem very portable, so I'll just use the basic versions.


