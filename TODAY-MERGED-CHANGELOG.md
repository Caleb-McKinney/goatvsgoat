# GOAT Court — Merged Update

This bundle combines the changes from today's build session into one upload set.

## Gameplay / presentation
- Stylized basketball avatars with stronger size differences.
- More basketball-like dribble, drive, shot, post, rebound, dunk and block poses.
- Player movement speed reflects mobility, so quick guards visibly separate from large centers.
- Dunk frequency is influenced by play style, athleticism, size, strategy and opponent rim protection.
- Dunks can miss or be blocked; they are never automatic.
- Dunk celebration with brief rim hang and GOAT Court logo burst.
- "FROM DEEP!" long-range celebration with follow-through, gold pulse, backpedal and retro sting.
- Retro synthesized SFX: bounce, sneaker squeak, swish, rim, block, steal, dunk, long-range sting, win/loss sounds.
- Original upbeat chiptune background music.
- Quick Sim / Skip to Result silences gameplay audio.

## GOAT Badges / Profile
- Daily qualified User Top 5 badge awards: 5 / 4 / 3 / 2 / 1.
- #1 also receives GOAT of the Day recognition.
- 5 badges -> +1 Ranked Play, max one Ranked badge redemption per GOAT day.
- 3 badges -> +2 Exhibition Plays.
- Dedicated Profile page.
- Rankings includes a Badges tab.
- Profile separates Overall, Ranked, Custom and Exhibition records.

## Custom Matchups
- User selects both legends from the 100-player roster.
- 3 free Custom Matchups per GOAT day.
- Guests can play without logging in; guest quota is stored locally on that browser/device.
- Signed-in Custom games save personal Custom + Overall records.
- Custom games never affect Elo, official legend rankings, User GOAT, Daily/All-Time ranked standings, or GOAT Badge qualification.
- Rankings includes a Custom tab for authenticated community Custom H2H totals.
- Guest Custom results are intentionally excluded from community H2H to reduce spam.
- Simulated Watch Ad button grants +2 Custom Matchups.
- Signed-in simulated ad grants use `grant_custom_ad_bonus()` in Supabase.
- The $0.99 / 24-hour unlimited Custom option is still UI-only until payments are integrated.

## Deployment
1. Replace the repo `index.html` with the `index.html` in this package.
2. Replace `game.html` too if your repo keeps it as a separate file.
3. Run `goat-court-badges-migration.sql` in Supabase if you have not already installed the badge schema.
4. Run `custom-matchups-migration.sql` in Supabase. This merged file includes the Custom Matchup tables/RPCs plus the simulated rewarded-ad grant RPC.

## Not included yet
- Real ad network integration.
- Real payment processing.
- The proposed preseason 50,000-game ranking seed. We discussed it, but it has NOT been run or added to production.
