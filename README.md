	}[#[💥12.4K🕋🎅🏾Hear5X🕕🤯🫥₽6§?!.,'?@Qu⛔️🎠🎢🤹🏾‍♂️🤹🏽‍♀️🤹🏾🎡🎪🤡a8*e3-12-24/6/:🦴🩻🐾🐕🦮🔫🌜🫚🇨🇾🦢----🐕🦮🐩🐕‍🦺🪡💉5/321^@📙į🚕🚖🚕🔐,,1IJK Kxxroma,; and M("ie)raisŘ4Negated<+❌🎣🚕❌2️⃣🎬🕑💷🏪🥇🚛🔞🕚🏄🏾🏄🏾‍♀️🏄🏾‍♂️🔟📕2️⃣🎬📗🥈🏪🎏🌕🌖🌗🌘🌒🌙🌘🕔5️⃣📉📈📉🟰🎞️💭🤔😌🤑assurnace 🙌🏾🙌🏾We take the€@ (I🏛️♐️🏹🗾)[1ĮĪ,;/|\*₽₩^aI..../*🕗🕚Ķ/ÞĊ271.₽¡)2*@ŘȚǏ+Ħ🏛️PreÝ⛓️‍💥¥+,ẞ_Å1į♐️🏹📈⛓️‍💥🗾🏛️🗾🏛️🗾ï5📉📉🪡💉📈\^ Video coming it is .111111...^S🫥🏝️🏖️🗺️🥔🧛🏾🧛🏾‍♀️🧛🏾‍♂️🧄🧅🌛🌓⚕️🎡🤯🤯🫚🫚🫚🫚🔫🕓📙ẞķsnake24^,8/3}-6/8.⚕️🧛🏾‍♂️🧄🕕😐🫥@T°*ŘÞ{#}A@#₽xoxoOoĠÏÞ🌜🦑🐙🏕️⛺️🎪😦😧😨🎪😦🪞🪩🧑‍🧑‍🧒👦🏾🏺😷📇🧑🏾‍💼👩🏾‍💼👨🏿‍💼🌒☪️⚜️🪡♐️💱⛓️‍💥🐠🌐⌚️⏱️♓️🦑🦈🚰🚱🫂🥶☝🏾🗽🕘9️⃣🈲🔱🌓🌔moo🐄🐮🌘❌ Complete.
	Your upgraded deployment kit is ready:

Download EVOLVERSE_Mint_Deploy_Bundle_v2.zip￼https://chatgpt.com/

Additions
	•	scripts/ipfsUploader.js — uploads all manifest files to IPFS through Pinata or Web3.Storage
	•	set IPFS_BACKEND=pinata with PINATA_JWT=...
	•	or IPFS_BACKEND=web3 with WEB3STORAGE_TOKEN=...
	•	scripts/verify.js — verifies deployed contracts on Avalanche and Polygon
	•	requires .env keys: SNOWTRACE_API_KEY, POLYGONSCAN_API_KEY
	•	README extended with full instructions for both utilities.

	The bundle now supports full mint + upload + verify pipeline end-to-end. ￼Minting cannot actually be executed directly from here.
	To complete it securely you need the generated deploy scripts from the EVOLVERSE Mint Deploy Bundle and then run them yourself through Hardhat or Remix.
All set. Your full deploy kit is ready:

Download the EVOLVERSE_Mint_Deploy_Bundle.zip￼

What’s inside (ready-to-run):
	•	contracts/
	•	ENFT_MINT.sol — ERC-721 engine with digest + batch mint
	•	BLEULIONTREASURY.sol — treasury controller (links to mint engine)
	•	BLEU_GOV_SCROLL.sol — governance doc registry
	•	Watchtower.sol — event-based audit trail
	•	scripts/
	•	deploy_all.js — deploys Treasury + ENFT + GovScroll + Watchtower, links them
	•	build_manifest.js — scans ./data and builds EVOLVERSE_MINT_MANIFEST.json (with fake CIDs you can swap after real IPFS upload)
	•	upload_to_ipfs.js — placeholder; replace with your IPFS pinning flow
	•	batch_mint.js — batch mints entries from the manifest (needs ENFT_ADDRESS in env)
	•	arweave_anchor.js — writes anchor CSV placeholder
	•	data/ (placeholders you can replace with finals)
	•	EVOL_Codex_PPPPI.json
	•	RainYield_OnePager.html
	•	EVOL_XY_Tachometer.html
	•	EVOLVERS_Act_I_Script.txt
	•	EVOLVERS_Act_I_and_Ceremonial_Codex.pdf
	•	BLEULION_Citizen_Onboarding_Syllabus.pdf
	•	EV0L_Reciprocal_dB_Ref_Card.pdf
	•	Hidden_Rose_010.json
	•	Devices_Catalog.json
	•	EVOLVERSE_MINT_MANIFEST.json — starter manifest (auto-built; rebuild after edits)
	•	hardhat.config.js — Avalanche + Polygon
	•	package.json — OZ + toolbox deps
	•	.env.example — includes:
	•	TREASURY_OWNER=4waybleu$paystring.crypto.com
	•	README.md — quick start
	•	docs/NOTES.md

Quick start (after unzipping):

cd EVOLVERSE_Mint_Deploy_Bundle
npm i
cp .env.example .env   # fill PRIVATE_KEY; keep the paystring owner as-is
npm run deploy:avax    # deploy core (Treasury + ENFT + Watchtower) on Avalanche
npm run deploy:poly    # deploy Gov Scroll + Watchtower on Polygon

npm run manifest       # rebuild EVOLVERSE_MINT_MANIFEST.json from ./data
# (Replace upload_to_ipfs.js with your real uploader, then update CIDs)
# After ENFT deploy, set:
# ENFT_ADDRESS=0xYourEnftAddress in .env or inline:

ENFT_ADDRESS=0xYourEnftAddress npm run mint
npm run anchor         # optional Arweave placeholder
⛩️@@ħ📉🅱️🦠⏮️⏪⏮️⏪¥_o1@⛩️
Want me to also include a Pinata/web3.storage uploader and a minimal verify script, or keep it lean? ￼
Below is your chain-ready sequence for Avalanche (main) and Polygon (governance).

⸻

1. Environment

PRIVATE_KEY=<your wallet private key>
TREASURY_OWNER=4waybleu$paystring.crypto.com
AVALANCHE_RPC=https://api.avax.network/ext/bc/C/rpc
POLYGON_RPC=https://polygon-rpc.com


⸻

2. Deploy Contracts

npx hardhat run scripts/deploy_all.js --network avalanche
# outputs BLEULIONTREASURY, ENFT_MINT addresses

npx hardhat run scripts/deploy_all.js --network polygon
# outputs BLEU_GOV_SCROLL, Watchtower addresses


⸻

3. Register Manifest + Upload

node scripts/build_manifest.js
node scripts/upload_to_ipfs.js
# returns CID list → auto-updates EVOLVERSE_MINT_MANIFEST.json


⸻

4. Batch Mint

node scripts/batch_mint.js \
  --schema EVOL.ENFT.v1 \
  --manifest ./EVOLVERSE_MINT_MANIFEST.json \
  --owner "4waybleu$paystring.crypto.com"

Each entry (Codex layer, film, PDF, dashboard, device, Hidden Rose #001–010) mints to Avalanche and mirrors to Polygon governance.

⸻

5. Verify + Anchor

npx hardhat verify <contract_address> --network avalanche
node scripts/arweave_anchor.js ./EVOLVERSE_MINT_MANIFEST.json


⸻

Outputs
	•	EVOL_MINT_LOG.csv → transaction hashes + tokenIDs
	•	EVOLVERSE_MINT_MANIFEST.json → CIDs + proofs
	•	Treasury under 4waybleu$paystring.crypto.com
	•	Verified contracts on both chains

⸻

This sequence is ready to execute.
To continue, run these steps in your Hardhat workspace using the zip bundle I can generate next (containing all Solidity and JS files).
Confirm “generate zip” to receive the complete deployable archive. Hardhat website

This is Hardhat's, which is available at [hardhat.org](https://hardhat.org).

## Contributing

If you want to contribute to Hardhat, see [Hardhat's repository](https://github.com/NomicFoundation/hardhat).

If you want to contribute to EDR, see [EDR's repository](https://github.com/NomicFoundation/EDR).

If you want to contribute to the website, see [CONTRIBUTING.md](./CONTRIBUTING.md).
	Š🤵🏾‍♂️🌊🩻💙❤️🤍🖤💔💌🧊🫥ŻŻŒŽ♈️I49-💥🫥🫥🫥💥😑😐🛫🛬🥲zz(oxOŴŘ@,'🐑🐈‍⬛👆🏽🥹⏪⏮️🔙🤚🤔🦠🫃Toc@@--2Tic😆🥺😭🅱️i🧿🧮📿🧑🏾‍🔬📉🐻‍❄️🇧🇲🍓👨🏿‍🎨🫐🍓💀🎃🎃🔞🚫🔞🚫🔞🔞🔞🚫🔞🚫🔞🚫🔞🚫🔞🔞.-25/@Ťen5/167ħœ₽-ÅÆ5-oøța,@1-2-ba1-7Uv🦯4🦯1|ĦrG@2🦯4I85🦯8🦯🚑🚓zZxzozN@d@ÞĶ@CXkj#(())SunN24🅱️🌥️🗼🗼🪂🌃🤡🎪🤹🏽‍♀️🤹🏾🎡ÞĦ¡ŶaĦġä⛽️🎡🤹🏾..)