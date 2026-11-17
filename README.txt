GANG NARCO ELITE V23

Included:
- Individual English personal signatures for all 12 members.
- Profile gift collection visual section (gift sending remains disabled until database/auth integration).
- Fixed bottom NARCO VOICE NETWORK panel with General Voice, Gang Meeting, Private Room and AFK Room.
- LiveKit browser SDK and client connection scaffold, including remote audio playback, microphone mute and leave controls. JOIN buttons intentionally remain disabled until a secure token service is configured.

VOICE ACTIVATION (required before members can use voice):
1. Create a LiveKit project and obtain its WebSocket URL.
2. Deploy a private token endpoint (for example, a Supabase Edge Function) that authenticates the signed-in member, checks room permissions, and returns a short-lived LiveKit access token in JSON as {"token":"..."}. Never expose LiveKit API secrets in index.html.
3. In index.html, set VOICE_CONFIG.livekitUrl and VOICE_CONFIG.tokenEndpoint in the NARCO VOICE CONNECTION script.
4. Serve the site over HTTPS and test microphone permissions, room membership, and moderation. The LiveKit browser SDK is loaded from jsDelivr.

The current static website has no shared authentication/database. Therefore profile gifts, persistent gift history, online member lists, and voice room presence cannot be made genuinely shared until backend/auth is connected. The voice interface is prepared but not falsely marked as live.

V23 update: repaired V17 CSS injection (previously rendered as visible page text) and refreshed the voice dock styling. Profile-related HTML and JavaScript were left unchanged. Voice connection still requires a configured LiveKit URL and secure token endpoint.

V23: profile popularity reactions (local preview), upgraded login and Hall of Fame styling, and 8 online instrumental sample tracks. Profile rendering and member click handlers retained from V21.

V23: tidied profile layout, refined member login panel, and added five playable online demo tracks to the audio queue.


V24: Announcement #002 and NARCO Support ticket prototype added. Ticket submissions are stored locally in the browser only; backend integration is required for management delivery.


V26 update: Added an in-page official YouTube video playlist with selected Persian rap and international hip-hop tracks. The player stays embedded on the site; availability can vary by region and video embed permissions.


V27: YouTube player removed. Direct MP3/device-file player retained; added direct licensed shuffle radio stream.
