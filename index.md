# Credentials

Name: Jacob Doan

Email: j5doan@ucsd.edu

Capstone Section: D17

Mentor: Tauhidur Rahman

# Prompts

## 1. What is the most interesting topic covered in your domain this quarter?

Simulating a drone in Isaac Sim. There is something fascinating about watching a robot you set up in simulation actually fly. The work (especially the setup with hardware compatibility and limitations) is long and often frustrating, but very fulfilling once you get a decent grasp of it.

What I enjoyed most was growing our pipeline bit by bit. At first, the goal was just getting Isaac Sim to run. Once we had Isaac Sim and Isaac Lab working, we built a simple pipeline that flew a drone from point A to point B. Each week we made it more useful, adding fault injection, outcome plots, batch runs and more. The moment that stood out was when we finally were successful injecting a fault into a flight run, such as one motor losing part of its thrust, and watching the controller try to recover.

## 2. Describe a potential investigation you would like to pursue for your Quarter 2 Project.

I want to investigate how we could add a higher-level AI layer that works alongside our trained PPO policies. The PPO policy would handle low-level control, keeping the drone stable even with a damaged motor, while the AI layer would handle higher-level decisions such as detecting which motor is failing, rerouting, or deciding when to land.

One open question is how the two should share control, since the PPO policy reacts many times per second while a larger AI model is much slower. We would compare this combined system against our Quarter 1 drones on recovery time, distance from the planned path and crash rate.

We also hope to test our best policy on a physical drone in the MOSAIC Lab. However, this depends on how well our policy performs in simulation, as well as the lab's budget and the hardware being developed by its PhD students. We see this as a long shot that might not even be feasible, rather than a planned milestone.

## 3. What is a potential change you’d make to the approach taken in your current Quarter 1 Project?

I want to collaborate more in sync with my teammates. The first few weeks were intentionally disjoint, because there is only so much that a team can do in the early stages. It only takes one person to build a working pipeline. A working pipeline had to exist before anything else could build on it. Others can only contribute as much by suggesting refinements to the experimental design, raising objections or new plans, reading papers to prepare for literature review, working on experiments to better understand their foundations of drones, or figuring out how to deal with their hardware limitations on running IsaacSim.

Now that we have a working pipeline and laid out the foundation of the experimental design, which consists of at least three experimental drones, we can split up the work and work in sync. The other person can handle other necessary miscellaneous tasks, such as updating the report, managing the team, making findings presentable, and running batch tests when available.

## 4. What other techniques would you be interested in using in your project?

I want to find more Claude skills that improve my development workflow and how I manage AI agents. This is my interpretation of an "approach" to our current project, not an experimental direction, to which I find more valuable in the long run. Examples that I discovered this quarter include graphify for mapping a codebase as a knowledge graph, caveman for shorter and cheaper agent reasoning, ponytail to make Claude behave like an extremely efficient and minimalist senior developer (cut more tokens), and guidelines based on Andrej Karpathy's advice on coding with LLMs.

I also want to spend more time writing detailed prompts in PLAN.md files and use plan mode more often, so the agent and I agree on an more refined approach before any code changes. Rather than being vague, it is good practice to be more specific and clear with your directions to get better results.

I'm also especially looking forward to building the project website, because it gives me a reason to try Claude skills made for UI/UX design.
