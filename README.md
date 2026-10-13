# Green Numbers, Red Signals – online ("Spot It First")

A single-page web app for the staged case **Green Numbers, Red Signals** (Omar, Senior Sales Executive).
One `index.html` file, no build step, no libraries. It runs on **GitHub Pages**.

The dashboard stays green all game. The groups are **not handed the signals**: they have to **choose where to look**, then every person **votes alone on their own phone**.

## Publish it on GitHub (5 minutes)
1. On github.com create a **new public repository**, for example `green-numbers`.
2. **Add file → Upload files**: drag in **`index.html`** (and `.nojekyll`), then **Commit changes**.
3. **Settings → Pages**: *Deploy from a branch*, branch **main**, folder **/(root)**, **Save**.
4. After 1–2 minutes the site is at `https://YOUR-USERNAME.github.io/green-numbers/`.
   (Pages on a private repository needs a paid plan, so keep the repository public.)

To change anything later, upload a new `index.html` to the same repository.

## Facilitator access
Open the site → **Facilitator** (or **Projector page**) → enter the code **2026**.
(To use another code, open `index.html` in a text editor and change `const FAC_PIN = "2026";`.)
This keeps casual visitors out; it is not strong security, because the code is inside the page file.

## How a stage works
- **Check-ins:** at each stage (2 to 5) a group has a few **check-ins** (3 by default, the whole group shares them) and **6 cards** to choose from, for example *Email activity*, *Calendar and working hours*, *Team meetings*, *Decision log*. A card **flips**: either it shows a **red signal** (one of the facts of the case) or **"Nothing new. It matches the dashboard."** Four or five cards hide a signal, one or two are decoys, and the groups can only open three, so **nobody sees everything**.
- **Timer:** a countdown (2 minutes by default) runs on every phone and on the projector. When it ends, the unopened cards lock.
- **Everyone in a group joins on their own phone** with the same group number. Flips are shared inside the group in real time.
- **Vote alone:** each person gives their own **concern level (1 = No concern … 5 = High concern)**. At Stage 4 they also tick the pattern they see (Energy, Connection, Efficacy) and at Stage 5 the work conditions (Workload, Control, Reward, Community, Fairness, Values).
- **Show results:** you press **Show results** and the vote distribution and the **signal wall** (who found what) appear on the projector and on every phone. **Reveal what nobody found** turns the dark tiles into the signals nobody looked for.

## Run a session
1. **Setup and group link**: a random **session code** is created for you (press *New session code* for every session). Choose the number of **check-ins** and the **time**, copy the **group link** and send it to the groups.
2. Everyone opens the link, picks the **group number** and presses **Join**. While waiting they read the case and the ground rule **"Describe observable changes only. Do not diagnose the person or use medical labels."**
3. Open **Stage 1** (the green dashboard). Everybody votes alone. Press **Show results**; ask *"What evidence supports your rating?"*
4. Open **Stage 2, 3, 4 and 5** one by one. Groups look around, vote, and you show the results and discuss. The **Trainer notes** (facilitator only) on the console give the prompt for the open stage.
5. Open **Final**: every phone shows **the full picture** (all 17 facts, marked *we found this* or *we missed this*). Everybody **votes again** and answers *"The dashboard is still green. Has your leadership response changed?"* Show results: the projector shows the first average, the new average and **how many people moved up**.
6. Open **Debrief**: the room's concern curve against the line that never left green, who spotted the most signals, **what each group never looked at**, and the closing message **GREEN NUMBERS. RED SIGNALS. Current output can stay high while the cost of producing it is rising.**

The **Projector page** follows whatever stage is open, so you can leave it on the big screen.

## Language: English / Arabic
- The top bar has a **العربية / English** button on every screen (including the join and facilitator pages). **Each person switches their own device**; the choice is remembered on that device.
- Arabic is **simplified Modern Standard Arabic** and the page flips to **right-to-left**. The core terms stay in English on purpose: Target, Capacity, Trust, Real Target, Energy, Connection, Efficacy and the work-condition words (Workload, Control, Reward, Community, Fairness, Values).
- In the facilitator console, **Copy Arabic link** gives you the group link with `&lang=ar` at the end, so a group opens straight in Arabic. (Any link can also be opened in Arabic by adding `&lang=ar` to it, or `&lang=en` for English.)
- Everything is translated: the screens, the case and cards, the buttons, the pop-up messages, the trainer notes and the debrief. The only thing that stays in English is the browser tab title until the page loads.

## Game feel and sound
Each stage opens with a full-screen splash, screens slide in, cards flip, coins drop when a check-in is used, the timer pulses in the last seconds and bars grow when results appear. Sound is made of short synthesized beeps and is **on by default on every screen**: press **Sound on / Sound off** in the top bar to turn it off (remembered on that device). Browsers only allow sound after the first tap on the page. Devices set to "reduce motion" get no animations or splash.

## How the live connection works
A website on GitHub has no server, so the app sends tiny messages (group, card, vote) through the **free public relay ntfy.sh**, on a private topic built from your session code. Because of that:
- Use a **new session code for every session**.
- The relay keeps messages for about 12 hours. Reloading a page rebuilds the session from them.
- If a phone is offline, it shows **Live sync: offline**. Each stage has a **backup 4-digit code** on your console that opens the next stage on that phone, but its flips and votes will not reach you.
- Please **rehearse once with two phones** before a live session.
- Advanced: open the site with `?relay=https://your-server/` to use your own ntfy server.

## Good to know
- Everything is saved in the browser of the device in use. *Reset session* clears the facilitator side (and creates a new session code); *Leave* clears a phone's group.
- The trainer notes and every hidden signal are part of the page code, so this is a classroom tool, not a secure exam. Phones only show the group pages.
- Check-in names (*Email activity*, *Decision log*…) were written for this app; the signals themselves are the facts from the case notes.
- You can test the app offline by double-clicking `index.html` (live sync needs internet).

Built for the Skills Bank "People First Leadership for Sales Leaders" programme.
