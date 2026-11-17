                                     _______.     ___       _______  _______ __     _______.
                                    /       |    /   \     /  _____||   ____(_ )   /       |
                                   |   (----`   /  ^  \   |  |  __  |  |__   |/   |   (----`
                                    \   \      /  /_\  \  |  | |_ | |   __|        \   \
                                .----)   |    /  _____  \ |  |__| | |  |____   .----)   |
                                |_______/    /__/     \__\ \______| |_______|  |_______/

 __________   ___ .______   .______       _______     _______.     _______. __  ____    ____  _______              ___       __
|   ____\  \ /  / |   _  \  |   _  \     |   ____|   /       |    /       ||  | \   \  /   / |   ____|            /   \     |  |
|  |__   \  V  /  |  |_)  | |  |_)  |    |  |__     |   (----`   |   (----`|  |  \   \/   /  |  |__              /  ^  \    |  |
|   __|   >   <   |   ___/  |      /     |   __|     \   \        \   \    |  |   \      /   |   __|            /  /_\  \   |  |
|  |____ /  .  \  |  |      |  |\  \----.|  |____.----)   |   .----)   |   |  |    \    /    |  |____          /  _____  \  |  |
|_______/__/ \__\ | _|      | _| `._____||_______|_______/    |_______/    |__|     \__/     |_______|        /__/     \__\ |__|

.______    _______ .______          _______.  ______   .__   __.      ___       __       __  .___________. __   _______      _______.
|   _  \  |   ____||   _  \        /       | /  __  \  |  \ |  |     /   \     |  |     |  | |           ||  | |   ____|    /       |
|  |_)  | |  |__   |  |_)  |      |   (----`|  |  |  | |   \|  |    /  ^  \    |  |     |  | `---|  |----`|  | |  |__      |   (----`
|   ___/  |   __|  |      /        \   \    |  |  |  | |  . `  |   /  /_\  \   |  |     |  |     |  |     |  | |   __|      \   \
|  |      |  |____ |  |\  \----.----)   |   |  `--'  | |  |\   |  /  _____  \  |  `----.|  |     |  |     |  | |  |____ .----)   |
| _|      |_______|| _| `._____|_______/     \______/  |__| \__| /__/     \__\ |_______||__|     |__|     |__| |_______||_______/


Welcome to the Readme for Sage's Expressive AI Personalities! What the fuck is this? I'll tell you what it ain't.

- It isn't made with generative AI, large language models, or any other automated bullshit. I made this by hand, like God herself intended. I drew the art, I wrote the dialogue, I made the code. Not even the thumbnail was made with AI, and everything I will ever make will adhere to those ethics. I explicitly do not consent to the inclusion of this code, or any part of any SEAP mod, in the use of any agentic training material or dataset. Fuck ALL the way off with that shit.
- It isn't to be distributed for-profit, at all, ever, for any reason. This shit's under the GNU license, respect it. You can use it, but you can't make people pay money for it. 
- It isn't meant to break the game or add massively complicated new mechanics. This is purely for immersion and roleplay, and it's going to stay that way.

So what _are_ Sage's Expressive AI Personalities?

SEAP (pronounced 'sheep') is a roleplay-centric dialogue overhaul that gives thoughtful, carefully crafted, expressive responses and behaviors to interstellar empires in Stellaris, the empire-builder sci-fi game by Paradox Interactive. Each AI Personality is intended to fill a niche that doesn't yet exist in Stellaris. These include greetings, declarations of war, offers to federate and subjugate, trade, and even insults. 

## What's in this Core ##
This core contains the necessary overwrites to make SEAP work. Whether you have hippies, pirates, or commies, all of them require the same set of overwrites in order to work. 
 - common/diplo_phrases
    These files overwrite vanilla greetings and agreements so that these unique personalities have their responses visible without messing with event weight. These files are load-bearing, and are unlikely to update (unless Paradox does something new).
 - common/diplomatic_actions
    Ethics and Civics Classic (SEAP's upstream dependency mod) uses a handful of unique diplomatic actions that are necessary for its mechanics to work as intended. The most complicated of these mechanics is the Primitive Player integration, which allows a player to play as a pre-FTL nation. Expressive Personalities may require a few changes to these hardcoded behaviors in order to reflect their personalities.
- common/game_concepts
    E&CC uses its own themed government civics, which have their own conflicts. SEAP tweaks these and adds its own unique class of themed governments, the Communal Parity. This is to fill in a bit of what I feel is an unbalanced mechanic. Communal Parity civics include Anarchy Utopia, Shared Burden, and Worker Co-Op.
- common/governments/civics
    Each civic has its own personality weight, which dictates how likely it is for a specific AI Personality to embrace a method of governance. Hippies are more likely to take environmentalist civics, and commies obviously will want to have Shared Burden or Labour Unions. This is included so that your Space Robin Hood neighbors don't suddenly become a police state for no reason.
- common/prescripted_flags
    Some of the prescripted nations included in SEAP's mods have their own unique introductions. This is to ensure that start screens appear correctly.
- common/scripted_triggers and common/scripted_variables
    In order to make these AI personalities exhibit certain important behaviors, like what fleet strategy they favor and whether they value xeno life, they refer to these scripted triggers. The most important trigger is 'is_special_personality', which dictates whether or not an empire has special dialogue in a given situation. Very important!
- gfx/portraits/asset_selectors and gfx/portraits/city_sets
    This is where the most time-consuming part of the mod is managed. The Diplomacy rooms that you see when you talk to an empire are controlled here. While this isn't wholly necessary, it does ensure that when a new DLC drops and Paradox has new furniture for your galactic takeover, I can keep up with the catalogue.

## Can I use this core for my own personality? ##
Hell yeah, go nuts!

## Is this hard to do? ##
Very. But it's doable.

## I don't wanna have a special line for every interaction. ##
You can always use $VANILLA_DIALOGUE_OPTIONS$ in localization to use stuff that's already in the engine. No shame in it if you're tired.

## Can you make X personality for me? ##
Nope! But you can. I'm a firm believer in the idea that if you want to see something made, you should be able to make it yourself. PDScript is very easy to learn, and while documentation is hard to find, the Stellaris Modding Den on Discord has some very cool and very experienced people who will gladly help you learn.

## I found a bug! ##
Report it here using Github, or reach out to me in the Discussion tab on Steam. I'll try and fix this as soon as I can.