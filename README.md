
# The automatic cinematic camera system for unreal with LLM
### Overview
- This is part of an AI-based 3D video generation initiative that uses the Unreal Engine.
- It focuses on abstracting the shot composition and directorial techniques commonly used in film theory.
- Utilizing shot definitions designed to align with human cognition and directorial theories, the goal is to leverage the capabilities of a large language model (LLM) to create a more natural camera timeline by specifying appropriate camera direction based on the scene's context.
- Additionally, it involves composing Shot Sequences and using them to build a MovieRenderQueue pipeline, as well as developing a CLI API to render LevelSequences through a Web API.

### Topics
<details>
  <summary>Shot parameter definitions</summary>
</details>
<details>
  <summary>AutoCamera, interfacing with LLM</summary>
</details>
<details>
  <summary>Implementing shot sequence generation</summary>
</details>
<details>
  <summary>Implementing MovieRenderQueue in CLI environment</summary>
</details>

### Issues
<details>
  <summary>Implemention of synchronous(blocked) HTTP request & process with response</summary>
</details>
<details>
  <summary>Motion blur issue when cut change timing in shot sequence</summary>
</details>
<details>
  <summary>Screen snapshot with full lumen illumination applied was required</summary>
</details>

---

# Updating MovieScene in UE5
### Overview
- This is part of an AI-based 3D video generation initiative that uses the Unreal Engine.
- With the transition from UE4 to UE5, the update mechanism for the SequencePlayer has become almost entirely asynchronous.
- Due to this, the ForceEvaluate, which was frequently used when computations needed to occur according to specific timeframes in the timeline, no longer performs the intended function (updating the scene). As a result, there was a need to find a solution for updating scenes in real projects.
- During this process, a positive side effect was the removal of the SetPlayPosition function, which had been habitually overused in the existing code.

### Topics
<details>
  <summary>Interrogator and constraint</summary>
</details>


### Issues
<details>
  <summary>The finalized animation update timing</summary>
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

### Topics

### Issues


---
# Others, misc.
- [Domain Setting Guide](https://github.com/dcode1119/DomainSettingGuide) - This page shows how to connect your domain to your github page(README.md)
- [WaveFunc](https://github.com/dcode1119/WaveFunc) - WaveExec.cpp shows how to generate a PCM wave format file.
