
# Cinematic camera system with LLM
### Overview
- This is part of an AI-based 3D video generation initiative that uses the Unreal Engine.
- It focuses on abstracting the shot composition and directorial techniques commonly used in film theory.
- Utilizing shot definitions designed to align with human cognition and directorial theories, the goal is to leverage the capabilities of a large language model (LLM) to create a more natural camera timeline by specifying appropriate camera direction based on the scene's context.
- Additionally, it involves composing Shot Sequences and using them to build a MovieRenderQueue pipeline, as well as developing a CLI API to render LevelSequences through a Web API.
- I was the key developer responsible for the core functionality of the cinematic camera system, utilizing Unreal Engine to design and implement the system.
- I thoroughly analyzed real cinematic works to ensure that the camera work in the system was both natural and effective.
- Through this system, I successfully integrated AI-driven camera movements into Unreal Engine’s LevelSequence, specifically within MovieScene, allowing for seamless and dynamic cinematography.
- This enabled the automatic insertion of camera work, emulating real-world film production techniques, enhancing the cinematic experience.

#### Issues & Topics
<details>
  <summary>Shot parameter definitions(WIP)</summary>
</details>
<details>
  <summary>AutoCamera, interfacing with LLM(WIP)</summary>
</details>
<details>
  <summary>Implementing shot sequence generation(WIP)</summary>
</details>
<details>
  <summary>Implementing MovieRenderQueue in CLI environment(WIP)</summary>
</details>
<details>
  <summary>Issue: Implemention of synchronous(blocked) HTTP request & process with response(WIP)</summary>
</details>
<details>
  <summary>Issue: Motion blur issue when cut change timing in shot sequence(WIP)</summary>
</details>
<details>
  <summary>Issue: Screen snapshot with full lumen illumination applied was required(WIP)</summary>
</details>

---

# Updating MovieScene in UE5
### Overview
- This is part of an AI-based 3D video generation initiative that uses the Unreal Engine.
- With the transition from UE4 to UE5, the update mechanism for the SequencePlayer has become almost entirely asynchronous.
- Due to this, the ForceEvaluate, which was frequently used when computations needed to occur according to specific timeframes in the timeline, no longer performs the intended function (updating the scene).
- As a result, there was a need to find a solution for updating scenes in real projects and found an explicit method and implemented it.
- During this process, a positive side effect was the removal of the SetPlayPosition function, which had been habitually overused in the existing code.

#### Issues & Topics
<details>
  <summary>  Interrogator and constraint(WIP)</summary>
</details>
<details>
  <summary>Issue: Considering the navigation system(WIP)</summary>
</details>
<details>
  <summary>Issue: The finali animation update timing was far later(PostEval)(WIP)</summary>
</details>

---

# Groupped action system
### Overivew
- This is part of an AI-based 3D video generation initiative that uses the Unreal Engine.
- This is a feature module that applies the animations of the entire project to characters through an Action System.
- It is a data definition used to insert and configure actions for various characters, targeting different timings or conditions as required.
- Since each individual group action has its own set of required parameters and execution timings, it was not feasible to design a single structure that could support everything.
- With this in mind, we approached the problem by considering each group action as a small scene that defines its content, and grouping them into Blueprints.
- Additionally, we wanted the actions to operate independently of any other calculations or custom logic.
- This Blueprint was developed as a plugin to be used as an Asset Type, and the data format could be operated solely through GameplayTags within the plugin.
- However, due to my departure from the project, I was unable to complete the development of the dedicated editor.
- Before the detailed planning phase, I was responsible for planning, designing, and verifying the Proof of Concept (POC) for the project.
- After successfully completing the POC, I handed over the project to the remaining team members, ensuring a smooth transition, and concluded my participation in the project.
- I hope that the project members who took over the POC work have applied it to the content creation features they immediately needed, and that it has provided them with inspiration to establish a foundation for better functionality.


#### Issues & Topics (WIP)

---

# Others, misc.
- [Domain Setting Guide](https://github.com/dcode1119/DomainSettingGuide) - This page shows how to connect your domain to your github page(README.md)
- [WaveFunc](https://github.com/dcode1119/WaveFunc) - WaveExec.cpp shows how to generate a PCM wave format file.
