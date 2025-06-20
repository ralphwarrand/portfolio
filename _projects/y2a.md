---
layout: project
title: "Year 2 Block A - Graphics Programming Exploration"
period: "September 2021 - November 2021"
tags: ["Graphics Programming", "Engine Architecture", "Team Collaboration"]
---

## Overview

[cite_start]This project, undertaken as part of the International Game Architecture and Design (IGAD) program at Breda University of Applied Sciences, focused on exploring the role of a graphics programmer within a team developing a retro 3D shooter engine.  [cite_start]The primary goal was to create a custom engine from the ground up, capable of running on both PC and PlayStation 4, with a special emphasis on learning the intricacies of graphics systems and cross-platform development.

**Key Focus Areas:**
* [cite_start]**Graphics Programming:** Gaining hands-on experience with graphics APIs and implementing rendering systems.
* [cite_start]**Engine Architecture:** Designing and building a robust, multi-platform game engine.
* [cite_start]**Team Collaboration:** Working effectively in a programmer-only team and communicating technical concepts.
* [cite_start]**Cross-Platform Development:** Tackling the challenges of developing for both Windows and PlayStation 4.

## Current State of Competency

[cite_start]At the start of this block, I had grown more confident in my general programming abilities since starting at BUas with no C++ experience.  [cite_start]I identified my strengths in communication within both programming-specific and multi-disciplinary teams.  [cite_start]However, I recognized that my organizational skills needed improvement and I aimed to become more reliable for future industry work.  [cite_start]My main goal for this block was to delve into graphics programming, as the mathematical concepts and visual results greatly interested me.

## Learning Goals

I set the following SMART goals to guide my development throughout the block:

* [cite_start]**Academic and Professional Practice Goal:** To improve my work-life balance by strictly adhering to assigned working hours and avoiding the overwork that occurred in the previous block.  [cite_start]I planned to measure my overtime hours weekly and actively work to reduce them.
* [cite_start]**Professional Skills and Knowledge Goal:** To explore the role of a graphics programmer by learning the foundational knowledge required for implementing rendering systems.  [cite_start]I planned to achieve this by creating a small demo project from scratch using either DirectX 12 or OpenGL during my self-study time.

## Weekly Progress Highlights

### Week 1: Team Formation and Initial Brainstorming
[cite_start]I was excited to be assigned to the Retro 3D shooter team.  [cite_start]A significant portion of the week was dedicated to brainstorming and planning the engine architecture with the team, which proved to be a draining but necessary process.  [cite_start]I also created a simple raycast renderer as a personal exercise inspired by the project.

![Brainstorming engine architecture on a whiteboard](assets/images/Y2A_W1_Brainstorm.png)
[cite_start]*Initial brainstorming session for the engine architecture.*

![Draft of engine architecture on a whiteboard](assets/images/Y2A_W1_Engine_Draft.png)
*Early draft of the engine's architecture on a whiteboard.*

### Week 2: Refining Engine Architecture and TDD
[cite_start]Our team made significant progress in outlining the engine's systems.  [cite_start]I learned more about the PS4's architecture, which helped in making our Technical Design Document (TDD) more relevant to our target platform.  We presented our initial engine design this week.

![Initial UML Diagram of the Game Engine](assets/images/Y2A_W2_Engine_UML_Initial.png)
[cite_start]*An early UML diagram showing the core components of the engine.*

![Final UML Diagram of the Game Engine](assets/images/Y2A_W2_Engine_UML_Final.png)
[cite_start]*The more detailed and final UML class diagram for our engine architecture.*

### Week 3: Project Setup and The Forge Integration
[cite_start]We successfully integrated "The Forge," a rendering framework, into our project.  [cite_start]A challenge this week was waiting for access to the PS4 version of the framework and our Perforce repository, which highlighted the importance of a solid initial project setup.  [cite_start]I also set up the FSL shader translation pipeline.

![Shader Translation Output](assets/images/Y2A_W3_Shader_Translation.png)
[cite_start]*Screenshot of the successful shader translation process.*

### Week 4: Getting the Project Running on PS4
[cite_start]A major milestone was getting our project to run on the PlayStation 4 for the first time.  I created an actor class and a model resource container. [cite_start]Feedback from our presentation indicated we needed to provide more concrete evidence of our progress and be mindful of project scope.

<video controls>
  <source src="assets/videos/Y2A_W4_PS4_Running.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>
[cite_start]*Video showing the project running on a PS4 for the first time.*

### Week 5: Asset Pipeline and JSON System
[cite_start]I implemented a system to load model resources from JSON files, which involved a significant restructuring of our asset folder.  [cite_start]This week reinforced the lesson that asset pipelines and folder structures should be established early in development.

![Asset Folder Structure](assets/images/Y2A_W5_Asset_Structure.png)
*The restructured assets folder, including JSON files for actors and models.*

![JSON Code Snippet](assets/images/Y2A_W5_JSON_Code.png)
*Example of the JSON structure for defining actors and models.*

### Week 6: Bug Fixing and Camera Rework
[cite_start]This week was dedicated to fixing numerous small but time-consuming issues, such as shader problems on the PS4 and default input bindings.  [cite_start]I also reworked the camera system, moving control to the player and adding cursor locking for the Windows build.

<video controls>
  <source src="assets/videos/Y2A_W6_Cursor_Lock.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>
*Demonstration of the cursor locking feature and updated camera movement.*

### Week 7: Fixing the PS4 Build and Cross-Platform Challenges
[cite_start]I spent this week fixing issues that had broken the PlayStation 4 build, which were primarily related to texture loading.  [cite_start]This was a challenging week as I was unwell, but it provided a deep dive into the complexities of cross-platform development and hardware differences.

![Project Running on PS4 Again](assets/images/Y2A_W7_PS4_Fixed.png)
[cite_start]*The project is up and running on the PS4 again after resolving texture issues.*

### Week 8: Final Presentation and Reflection
[cite_start]The final week was focused on completing the Intended Learning Outcomes (ILOs) and preparing for the final team presentation.  [cite_start]The feedback confirmed that we had over-scoped the project, a key lesson for future endeavors.

## Block Reflection

This block was a significant learning experience. [cite_start]I am proud that our team created a 3D game engine in just eight weeks and that I was the primary person responsible for the PS4 implementation.  [cite_start]One of the biggest challenges was working with "The Forge" framework due to its limited documentation.

The most important lesson I learned was the danger of over-scoping. [cite_start]In the future, I will advocate for creating a smaller, more polished experience first and then building upon it.  [cite_start]I also learned the critical importance of detailed planning in the initial stages of a project to avoid on-the-fly decision-making.  [cite_start]While I enjoyed my role as a Graphics Programmer, I also found myself heavily involved in gameplay and engine programming, and I am still exploring which specialization I enjoy the most.

## Technical Skills Developed

-   **Programming Languages**: C++
-   **Graphics APIs**: DirectX 12, PSSL (PlayStation Shader Language)
-   **Tools & Frameworks**: The Forge, Perforce, Visual Studio
-   **Methodologies**: Agile development, SMART goal setting, Technical Design Document (TDD) creation
-   **Collaboration**: Multi-disciplinary teamwork, Discord for communication, technical documentation

## Key Takeaways

This block provided valuable experience in graphics programming, engine architecture, and team collaboration. It was a challenging but rewarding journey that significantly contributed to my growth as a game developer and better prepared me for the complexities of the industry. The hands-on experience with cross-platform development for the PS4 was particularly invaluable.

---

*This project page is part of my ongoing portfolio documentation. For more details about specific implementations or to discuss this work, feel free to [contact me](mailto:contact@ralphwarrand.dev).*