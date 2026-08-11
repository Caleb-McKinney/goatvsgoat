# v28.3 Simulated Rewarded Ad Test

1. Open Custom Matchup while signed out.
2. Confirm 3 free guest games.
3. Tap "Watch Ad → +2 Custom Games".
4. A simulated 1.2-second ad delay runs, then +2 games are added.
5. Guest bonus persists for the current GOAT day on that browser/device.
6. Sign in and repeat. Signed-in users receive +2 through the `grant_custom_ad_bonus()` Supabase RPC.
7. The button can currently be used repeatedly for beta testing. We can later cap rewarded ads per day.
8. Guest ad bonuses do not affect rankings/community stats; they only increase guest Custom quota.
