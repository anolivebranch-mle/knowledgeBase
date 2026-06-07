# Moderation Processing Guide

Note on snippets: They use spaces to determine arguments. If the player’s name has spaces in it, make sure not to include the spaces!

## Ticket Intake

Moderators do not see the new tickets category. New tickets will have to be moved to the moderation category by LO/Community/Coordinator+

Upon receiving a new ticket, a lead moderator will be assigned and pinged. Find the lead mod in the mod-rotation channel. The lead moderator will be responsible for communication with the reporter, prompting discussion about the case, creating the poll, and taking action on the specific case if deemed necessary.

1. Use the !!modreport snippet to acknowledge the player’s report
    1. Usage: “!!modreport {playername}”
        1. Do not include spaces in the player's name.
    2. If we receive a ticket with no information please tell the reporter something like, “You are with moderation now, please let us know how we can help you.”
2. Ping the lead mod and begin a discussion of the provided report
    1. You can also ping all mods to start the discussion
3. LEAD MODERATOR TAKES OVER CASE
4. Once discussion seems to be leaning towards a decision, please create a poll to vote on a decision for the specific case.
5. Voting should consist of the following:
    1. Ping moderator role
    2. Provide several of the decision options that were discussed during the investigation
    3. Provide an “other” option, to allow for more discussion if necessary
6. Execute whatever decision was made

## Decision Execution

### No Evidence Reports

1. Log the warning in the #no-evidence-reports channel in the MLE Staff server
    1. Search their Discord ID in the main discord server.
    1. Refer to previous reports in the channel for an example of proper formatting.

### Informal Warnings

Informal warnings do not add any points to the user’s record, do not count against the mod point reset cooldown, and do not go through the bot. We use the staff mailbox to send a message

1. Write up the warning. We do not have a formal format, but there’s a bit of a precedent
    1. ```Hello {playername}, it has come to our attention that you {insert action from player that report resulted from}. This kind of behavior is not tolerated in MLE. This is just a warning, no points have been added to your record.```
        1. ``` These are called backticks and help with visuals and copy/paste
        2. {} Remove the brackets
2. Be sure to have another member of the Moderation team double-check the warning text.
3. Once the warning text is decided, open a mailbox ticket with the reported user
    1. !newthread {discord ID}
    2. Someone who has access to new tickets will need to move it to the moderation category
4. Ensure that your mailbox role is set to “Moderator” (applies to those with a higher staff role than mod, such as coordinator)
    1. Use “!role moderator” in the ticket
    2. Check your current role with “!role”
5. Send the warning text to the user anonymously
    1. Use “!ar {warning text}”
6. Log the warning in the #informal-warns channel in the MLE Staff server
    1. Refer to previous reports in the channel for an example of proper formatting..
7. Give the ticket at least a day for any response before closing it out
    1. You can send snippets anonymously by using 3 !s. Use “!!!close”

### Non-Ban Warnings

1. Get how many points the person already has. This information is in the “Print Sheet” tab of the mod tracking sheet
    1. Remember when getting the final punishment, it will be based on the new total points, not just points added this infraction

2. Write up the warning. The format is in the “Example Warn” tab of the tracking sheet
    1. Make sure there is a space after the user’s discord ID
    2. Date should be the date they violated the rule
    3. Infraction text should be what they said, unless that would give away the reporter, in which case, make it more generic. Judgment call
    4. Rule num - Rule text pulled straight from rulebook
        1. Example: 1.3 - Using racist/homophobic/ableist/misogynistic/pedophilic/xenophobic remarks
    5. Rule level - number of points
    6. Rule point violation text - pulled from rulebook
        1. Example: Making moderately racist/homophobic/ableist/misogynistic/pedophilic comments or remarks
    7. Rule punishment - straight from rulebook
        1. CHECK FOR PROBATION PERIOD, if last join date was within 90 days, 3+ points is a ban
3. For multiple violations, list each separately within the warning, for example
    ```
    This content violated Rule **1.3 - Using racist/homophobic/ableist/misogynistic/pedophilic/xenophobic remarks.**
    This violation was a Level **5** violation for **Making moderately racist/homophobic/ableist/misogynistic/pedophilic comments or remarks**. 
    This content also violated Rule **1.1 - Insulting another person or group of people.**
    This violation was a Level **2** violation for **Comments that are moderately insulting**.
    ```
4. Have another mod double check the warning text
5. Once decided, submit it in the mod tracking form
    1. MLE ID can be found in a few ways. Pull up the user in the print sheet page of the tracking sheet. Find one of their salary cards. Go to the player directory
    2. Moderators should be those who were involved in discussion. Advisors/directors/board do not need to be included in this
    3. Player action should be what they did. This will only be seen by mods
    4. Official response should be a copy and paste of the full warn command
6. Warning/mute commands should go in the #warden-commands channel in the staff server
	1. Do /warn and it will give you a popup where you can enter the discord ID and warn text.
	    1. IMPORTANT NOTE: There is a known bug with the bot where the warning text CANNOT be longer than 1024 characters
    2. 0 point warnings
        1. Send the warn command
    3. 1 and 2 point warnings
        1. Send the warn command
        2. /mute (discord ID) (time, 7d for 1pt, 14d for 2pts)
        3. /mute 222809044103069696 7 days
    4. 3 and 4 points (assuming not on probation)
        1. Coordinate with LO to establish a 1 or 4 week league play suspension
            1. If the player is on a franchise, make a ticket with the GM and FM in joint mod lo. Format and example in the snippets channel in mailbox server
            2. Ping LOTM in the staff server #mod-lo coordination
                1. Give them the player name, MLEID, Length of suspension, and what rule was broken.
        2. Coordinate with community team to ensure any existing staff positions are vacated
        3. Send the warn
        4. /mute (discord ID) 28 days
    5. 5 points and 3+ while on probation, see below

### Bans

1. Follow steps for a non-ban warning, DO NOT send the warn command yet
2. Write the ban announcement
    1. Template:
    ```
    [player name] has been banned from MLE for accumulating 5 or more mod points.
    They violated rules:
    [rule num + text] (do not include rule level or rule level text)
    ```
    2. Probation Template:
    ```
    [player] has been banned from MLE for accumulating 3 or more mod points while on probation.
    They violated rules:
    [rule num + text] (do not include rule level or rule level text)
    ```
    3. Example:
    ```
    AlyssaBee has been banned from MLE for accumulating 5 or more mod points.
    They violated rules:
    1.1 - Insulting another person or group of people
    1.12 - Unsportsmanlike conduct within the MLE Community
    ```
3. Coordinate with LO to move the player to FP (Former Player)
    1. Not necessary if the player is already FP
4. Ping @Director to get someone ready to execute the ban
5. Once they are ready, send the warn command through the #warden-commands channel of the MLE Staff Discord server
6. Once the warn goes through, give Director+ the green light to ban the player
    1. Make sure to specify the **player**’s Discord ID (reporters have accidentally been banned in the past)
7. Once the ban has occurred, make sure to have Team Lead+ send the ban announcement in #community-announcements of the MLE Discord Server

## Ticket Resolution

1. Once appropriate action has been taken, please begin the process of closing a ticket.
2. Use the !!modcloser snippet to tell the reporter that their case has been handled
3. Set a scheduled close for several hours. We do this so that other moderators have time to see things before the ticket closes.
!close 6h
4. If any tickets are open with FM/GMs, please schedule those with several hours before closing too.
5. NOTE: If you accidentally opened a ticket, please use the silent close command “!close s 3h”
