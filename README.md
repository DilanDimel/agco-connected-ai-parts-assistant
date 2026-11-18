# AGCO Connected AI Parts Assistant — Concept Prototype

A clickable prototype for our INSC 20263 Digital Transformation Consulting project (TCU, Fall 2026), by Team Tantalizing Table Two: Dilan Desman, Wesley Taylor, and Samson Romano.

**Live demo:** https://dilandimel.github.io/agco-connected-ai-parts-assistant/ (GitHub Pages)

## What the project is about

Parts make up about 19% of AGCO's net sales, but today the farmer parts journey is reactive. A machine breaks, the farmer calls or drives to the dealer, the dealer looks up the part by hand, and then checks dealer stock and AGCO stock in separate systems.

We propose a **Connected AI Parts Assistant** inside the FarmerCore app with three parts:

1. **AI photo part identification**: the farmer uploads a photo and serial number. The AI suggests the part and shows how confident it is.
2. **One live availability check**: dealer and AGCO warehouse stock are checked together, and backorder date changes are sent to the farmer automatically.
3. **Fault-triggered alerts**: AGCO Connect tractors that report a fault code start the parts request before the farmer calls.

Humans stay in control. Dealers can reserve only when the AI is at least 80% confident and the part is in stock. Anything else goes to a parts specialist.

## What's in the prototype

- **Overview**: the problem, the solution, human-in-the-loop rules, hybrid-cloud architecture, benchmarks, roadmap, costs, and sources.
- **Farmer app**: a phone mockup with a fault alert, photo scan, AI result, and order tracking, plus a live "behind the scenes" event feed.
- **Dealer desk**: a request queue with the AI suggestion, a one-check inventory view, decision rules, and reserve, warehouse-order, and escalate actions with an audit log.

## Run it

Open `index.html` in any modern browser. There's no build step and no backend.

## 60-second demo script

1. Farmer app → **Start parts request** from the tractor's fault alert.
2. **Scan part** → choose the worn drive belt → **Identify**. The AI is only 62% sure → send it to the dealer.
3. Dealer desk → reserve the 96% DPF sensor, then escalate the 62% belt.
4. Back on the Farmer app, check the push notification and the Orders tab.
5. Click **Simulate: warehouse moves up ETA** to see an automatic backorder update.

## Disclaimer

This is a student concept demo. All data is simulated. It is not affiliated with or endorsed by AGCO Corporation. The part and field photos are AI-generated.
