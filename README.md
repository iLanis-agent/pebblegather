# Pebblegather 1.0 TEST

Native Android Hiroimono disappearing-stone puzzle. Android 8+ (min26), target35. Package com.gg007.pebblegather.

## Rules
Hiroimono with a fixed first stone. S is already picked up. Use UP, RIGHT, DOWN or LEFT to travel along a grid line to the nearest remaining stone and pick it up. You cannot skip a stone. After that, continue straight or turn 90 degrees; never make a U-turn. Direction changes happen only when picking up a new stone. Collected positions are empty and may be passed through again, without turning there. Gather all eight stones. Twelve unique 4x4 stone patterns with twelve distinct unique solution routes. Every solution passes a previously collected position and continues straight at least once. Undo/reset/next/level selection and saved stone palette/pickup-number settings.

## Download and status
https://mega.co.nz/#!gYNFESBD!dN_sXTivaQ_NXMrpsxtXr-CscVLV4q1rYxldv11o-yg
APK SHA256 4639bf2c4763dbac8881067aa49e39c055397a33abb97a9eee802ca052c2c2d0; 16878 bytes. Original signing certificate SHA256 1651d9e269ece8a76f36ed4bba24ebc50f9de1e5f856e0567e0e8169fcb25597. Anonymous download bytes match.

Independent Java aligned-candidate collection and distance sorting agrees with production stepwise ray search on all983040 combinations of remaining-stone subsets, current positions, previous direction and requested direction across twelve boards. This includes unreachable and invalid position/subset states. Independent DFS confirms exactly one route per fixed start. Twelve distinct boards and routes. Bounds, invalid direction/position/previous inputs, solved-input lock, solve, undo to start and replay pass. Actual archived generator regeneration and archived Java tests pass. Drawing-adapter controls, saved settings, privacy, completion marks, next and level selection pass. Actual game/menu/settings/privacy/levels/solved drawing pixels inspected, not phone screenshots. Phone runtime, performance and external browser handoff QA remain incomplete. Signed TEST only, not final and not Play published.

## Functional difference
Live803-entry registry,118 recovered partial README records and semantic review of all144 cards in the exact Heronputt cumulative stage found no Hiroimono/Goishi Hiroi match. Cindertrail takes single-cell steps to gather three sparks without revisiting tiles. Pebblegather jumps to the dynamically nearest remaining stone, removes it from future line-of-sight stops, permits passing collected positions, and bans U-turns. Heronputt uses fixed decreasing shot distances, permanent blocked trails and holes; this uses disappearing targets and no reserved trails. Nightstride uses fixed chess-knight leaps to visit lit cells. Known Hiroimono genre, not a global invention. Corpus is partial. Rules verified at https://en.wikipedia.org/wiki/Goishi_Hiroi and https://www.keepitsimplepuzzles.com/how-to-solve-hiroimono-puzzles/ with fixed-start variant also defined by https://www.brics.dk/RS/07/1/BRICS-RS-07-1.pdf .

## Build
JDK17 and Android SDK platform35/build-tools35.0.0. Run python generate-levels.py to reproduce levels.json. Board.java embeds the generated stone masks, fixed starts and solutions. javac -d /tmp/pebble-test src/com/gg007/pebblegather/Board.java BoardTest.java and java -cp /tmp/pebble-test com.gg007.pebblegather.BoardTest. bash build.sh builds an unsigned aligned APK unless KEYSTORE_PATH and KEYSTORE_PASSWORD_FILE point to private original signing inputs. No credentials in source. Release build settings, signed TEST artifact, not a final store release.

## Privacy and branding
Pebblegather runs offline without accounts, ads, analytics, third-party SDKs or requested permissions. Stone palette, pickup numbers and completed-puzzle marks stay in the app on your device. Clear app data or uninstall to remove them. The studio link opens your external browser.
GG007 icon copied byte-for-byte from preserved original. Menu includes studio https://ilanis-agent.github.io/gg-007-gaming/ and privacy.

## Preservation
Complete source and APK privately preserved at https://files.instinct.com/2mgzujh9p7iv-pebblegather-source-archive with exact cumulative staged HTML. GitHub https://github.com/iLanis-agent/pebblegather holds README only; full Git source commit remains pending. Cumulative stage is NOT LIVE; existing studio run remains queued. No Pages settings changes, rollback or Play rollout. Updated November 7, 2026.
