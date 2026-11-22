# D–H Classroom Lab — Interactive Modified Denavit–Hartenberg Activity

A self-contained, responsive learning website for teaching robot kinematics. This repository contains the **Version 13** R–R–P classroom activity. It is suitable for laptop, tablet, and mobile browsers.

**Classroom website (once Pages is activated):** https://akhoshiar.github.io/dh-classroom-lab/

## What students can do

- Manipulate an R–R–P serial robot in an interactive **3D / Top / Side** view.
- Add or remove revolute and prismatic joints and adjust link lengths.
- Choose the directions of each frame's **z-axis** (joint motion axis, red) and **x-axis** (common perpendicular, green).
- Check their choices and read rule-based feedback.
- Complete the **Modified D–H** table (a_(i−1), alpha_(i−1), d_i, theta_i), check their entries, and optionally reveal the instructor solution.
- Consult the D–H rules and parameter definitions at the bottom of the page.

The default exercise starts with a three-joint **R–R–P** mechanism and four physical links. An optional six-joint example is included.

## Enable GitHub Pages (one-time setup)

The website source is already committed to the public repository [akhoshiar/dh-classroom-lab](https://github.com/akhoshiar/dh-classroom-lab) on the `main` branch. No installation or build process is required.

1. Open [Settings → Pages](https://github.com/akhoshiar/dh-classroom-lab/settings/pages).
2. Under **Build and deployment**, choose **Deploy from a branch**.
3. Select **main** and **/(root)**, then click **Save**.
4. Once GitHub reports the deployment is ready, share [the classroom site](https://akhoshiar.github.io/dh-classroom-lab/) with students.

See [GitHub's documentation](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site).

## Run locally

Open `index.html` in a modern browser. No npm installation, build tool, server, or API keys are required. For local HTTP testing, run `python -m http.server 8000` from this directory and visit `http://localhost:8000/`.

## Classroom use and privacy

This is a **static client-side website**. Student answers and grading are processed in the browser. The app has **no server-side login, database, or central collection of student scores**. If you need to collect submissions or track marks, that would be a separate feature (e.g. a connected learning platform).

The displayed instructor solution uses a chosen consistent D–H sign convention; where alternative frame assignments are valid, their numerical D–H parameters may differ. Students should follow the displayed exercise convention or rederive the table consistently.

## Project files

- `index.html` — complete interactive application, including HTML, CSS, SVG and JavaScript.
- `.nojekyll` — publish files directly, without Jekyll processing.
- `README.md` — project introduction and publishing instructions.

## Updating the deployed app

Change `index.html` and commit the updated file to the `main` branch. GitHub Pages will redeploy it automatically. Keep the file name `index.html` so the main URL opens the exercise.