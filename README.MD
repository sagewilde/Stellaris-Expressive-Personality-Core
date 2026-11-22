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
    In order to make these AI personalities exhibit certain important behaviors, like what fleet strategy they favor and whether they value xeno life, they refer to these scripted triggers. The most important trigger is 'is_seap_personality', which dictates whether or not an empire has special dialogue in a given situation. Very important!
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

Thanks for opening the Readme! Here are my notes on making this mod.

## I wanna make a personality like this! ##
I figured you were going to ask that. Here's what you need to do.

1- Start with a script. No, not a code script (unless you want to do that), I'm talking about an actual script for character dialogue. How does this empire want to be perceived by the galaxy? Think very carefully about the kind of image you want to project here. 
! Remember, if their civics, ethics, or government form changes, depending on how you key their personality, it could obliterate all the dialogue you have planned. If you can, try to key the personality requirements to something that can't change later in the game, like the Chosen civic, or a species portrait.
! Don't try to skip out on work and only write a few lines. The way that the diplo-phrases files I wrote work, you'll have to deal with replacing EVERYTHING. You can always key default phrases in vanilla $using_dollar_quotes_like_this$, but you do still have to make a MYPERSONALITY_GREETING_01 statement. 
! Relax, and take your time. Writing is hard work. And it's worth it to do it on your own, with your own brain. If you rush it, it'll come out like crap.

2- Decide how you want this personality to behave.
As you've noticed, the Hippies and both of the Pirates have specific behaviors related to their personalities. That back-end functionality is difficult to maintain because it requires overwriting code in blocks frequently used by other mods. If you don't stay on top of things like updates and patches, you could end up breaking a lot of things without meaning to. The only reason I touch as many files as I do is because I'm one of the maintainers of E&CC. I know what changes are coming down the line, so I can prepare for them.
! Avoid editing load-bearing files like ethics.txt or civics.txt unless you know you can maintain this mod, know what changes are happening, or otherwise know what you're doing.

3- All hail the almighty, all-wise KISS... Keep It Simple, Stupid.
This is a rule I need to remember to follow more often. When you keep a task simple, you're setting yourself up for success. The more complicated it becomes, the more likely it is to break. As awesome as it would be to have this empire have a specific catch-phrase that they say only with empires that have this specific civic after they've developed this specific technology, that's involving a lot of conditions, triggers, and otherwise iffy variables that your players might not even see. Ask me how often I've had players encounter Hippies that have successfully made the Planetary Shielder colossus.

4- The files you need to write.
Here's all the stuff you need to get your own Expressive personality working:
 - common/personalities/sample_personality.txt
 - common/diplo_phrases/sample_diplo_phrases.txt
 - common/diplo_phrases/sample_greetings.txt
 - common/diplo_phrases/sample_greetings_nomad.txt
 - common/scripted_triggers/sample_scripted_triggers.txt (more later)
 - localisation/klingon/sample_basic_l_klingon.yml
 - localisation/klingon/sample_greetings_l_klingon.yml
 - localisation/klingon/sample_greetings_nomad_l_klingon.yml
 - localisation/klingon/sample_phrases_nomad_l_klingon.yml

If you're using my files to make your personality, you need to add your own entry to the is_seap_personality trigger, replacing 'seap_sample' everywhere you find it mentioned.

    is_seap_personality = {
	    OR = {
		    has_ai_personality = peaceful_counterculture
		    has_ai_personality = mirthful_bandits
		    has_ai_personality = cunning_raiders
            has_ai_personality = seap_sample
	    }
    }

What this does is it tells the overwritten diplo-phrases files that your personality has its own dialogue, and it should ignore it when presenting dialogue in the diplomacy window. When you do this, you're going to have to make sure that you have a proper dialogue entry for every article in 00_diplo_phrases_02.txt, 00_diplo_phrases_nomads.txt, and (if they are or can ever be a megacorporation) 00_corp_greeting_overwrites.txt.

Everything after that is localisation. And trust me, it's a hell of a lot harder than it looks. If you're localizing in English (my native language), you have it pretty easy. If you're localizing in other languages, you may have to look for extra help to make sure that your super-cool AI personality is using good grammar.

For any localisation, you need a text file that is saved with a '.yml' extension. YAML is short for Yet Another Markup Language, and it's what the Clausewitz engine uses to read loc files. You can write one in any text editor that isn't Microsoft Word or LibreOffice Writer. But, you need to make sure that you're saving the file with UTF-8-BOM encoding, which is short for 'Universal Text Format 8, with Byte-Order Markup'. Otherwise, Clausewitz won't know what to do with it. The sample locs have all of that set up, so you can jump right in and just start going for it.

Make sure that your localisation file has 'l_klingon: ' written on the very first line and nothing else (substituting 'klingon' for your native language, unless you're actually a Klingon). And, every single line after that MUST have a single space at the start, or else it won't work. Your loc files should ALWAYS end with the language they're written for, and should be in their proper folder.

    /mod/MyAwesomeSEAPPersonalityMod/localisation/klingon/sample_l_klingon.yml

If you're replacing text that's anywhere in any other file in the vanilla game, then you need to put it in a folder named 'replace'. If you don't do this, you will make the game crash before it loads. I'm telling you now to save you a lot of pain later on, so ignore my warning at your risk.

    /mod/MyAwesomeSEAPPersonalityMod/localisation/klingon/replace/sample_overwrites_l_klingon.yml


For your own sanity, here's a template for you:

l_klingon:
 #Greetings
 XX_FRIENDLY_GREETING_01:0 ""
 XX_NEUTRAL_GREETING_01:0 ""
 XX_HOSTILE_GREETING_01:0 ""

Everything should, more or less, look like that. Yes, the zeroes are necessary for English. No, I don't know why, I taught myself how to do this through trial and error, so no one's explained it to me. As long as all your loc files have their proper language name in the first line and at the end of the filename, you can name them whatever you like. I use this to organize them so I know what's in each file.


## Why did you make such a stupid mod? That's a lot of effort for one dumb joke. ##

You're damn right it is, and I still think it's hilarious.

When I first downloaded Ethics and Civics Classic, I decided that it would be really funny to make a Fanatic Pacifist-Ecocentrist empire. When I found Cybrxkhan's monstrously huge namelist and saw the Space Hippies on it, I quickly found my favorite roleplay empire. I found myself cracking dumb jokes with no audience. I decided that it was amusing enough that someone else would have found it funny. So, I just... kinda did it. Everything after that is pretty much history.

That's pretty much it.
