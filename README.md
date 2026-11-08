# Balancecress 1.0 TEST
Native Android Balance Loop. These small boards are original generated layouts. Android 8+ (min 26), target 35. Package com.gg007.balancecress.

## Rules
Balance Loop. Draw one closed, noncrossing, unbranched loop on orthogonal cell-center edges, visiting every circle. Unused plain cells are allowed. From each circle measure both straight arms, in edges until the next turns. Other circles do not stop the count. White circles need equal arms; black circles need unequal arms. Each printed number is the sum of both arms. Either color may go straight or turn on its circle. All clues in this edition are numbered. Tap gaps between centers to add/remove road edges. Twelve original unique 4x4 clue boards with twelve different completed loops. Undo/reset/next/levels and saved loop palette/equal-unequal labels.

## Download and status
https://mega.co.nz/#!oJdDCIrJ!CCTBNCG3SVepiZWJ8n9rxFQTlRuE9CCgV-95G8AfEzw
APK SHA256 b58ae6b9a69f741bf19e451f5dbd92f3e14c378123cd5f7434b7ac2a26fdf98f; 20974 bytes. Original signing certificate SHA256 1651d9e269ece8a76f36ed4bba24ebc50f9de1e5f856e0567e0e8169fcb25597. Anonymous download bytes match.

## Checks
Original portable generator enumerates all 213 simple cycles on a 4x4 cell-center grid and creates twelve uniquely constrained original boards. Independent Java ordered-cycle tracing agrees with production degree/BFS topology on ALL 16,777,216 edge masks. Independent ordered-coordinate arm runs agree with production neighbor-vector stepping on all 213 loops for all twelve boards; each has exactly one solution. Another 120,000 random/invalid clue-mask cases, 288 single-edge solution mutations, bounds, solved lock and solve/undo/replay/reset pass. Archived generator reproduces levels.json and all-cycles.json byte-for-byte; archived Java passes. Drawing adapter tests actual road taps, undo/replay/next/levels/menu/settings/privacy and saved palette/equal-unequal labels/completion. Six drawing screens inspected, not phone screenshots. Phone runtime, performance and external-browser handoff QA remain incomplete. Signed TEST, not final or Play published.

## Functional difference
Live 803-entry registry and semantic review of all 163 prior studio cards found no Balance Loop match. Signalfern (Shingoki) forces white circles straight and black circles turning; Pearlmere (Masyu) has neighboring-turn rules; Runebriar (Geradeweg) assigns segment lengths. Balancecress instead makes circle color compare equal or unequal straight arms, with either color free to turn or go straight. Known Balance Loop genre by Prasanna Seshadri, not a global invention. Primary rules https://www.gmpuzzles.com/blog/balance-loop-rules-info/ explicitly define this difference. No source puzzle copied; original generated clue boards. Recovered repository corpus remains partial.

## Build
JDK 17 and Android SDK 35/build-tools35.0.0. python generate-levels.py reproduces levels.json. Board.java embeds generated circle-color/sum clues and road solutions. javac -d /tmp/balance-test src/com/gg007/balancecress/Board.java BoardTest.java and java -cp /tmp/balance-test com.gg007.balancecress.BoardTest. bash build.sh creates an unsigned aligned APK unless KEYSTORE_PATH and KEYSTORE_PASSWORD_FILE point to private original signing inputs. No credentials in source. Release build settings, signed TEST artifact, not final store release.

## Privacy and branding
Balancecress runs offline without accounts, ads, analytics, third-party SDKs or requested permissions. Loop palette, equal-unequal labels and solved-board marks stay in this app on your device. Clear app data or uninstall to remove them. The studio link opens your external browser.
GG007 icon byte-equal to original. Menu studio https://ilanis-agent.github.io/gg-007-gaming/ and privacy.

## Preservation and websites
Complete source and APK privately preserved at https://files.instinct.com/u19qh6mn9by1-balancecress-source-archive, including exact cumulative 164-card studio and published catalog/studio sources/updater. Repository https://github.com/iLanis-agent/balancecress holds README only; full Git source commit pending. Both website publications checked separately. No Pages settings change or Play rollout. November 8, 2026.
