
# List of contents

---

### An automatic cinematic camera system for unreal with LLM
##### Overview
- This is part of an AI-based 3D video generation initiative.
- It focuses on abstracting the shot composition and directorial techniques commonly used in film theory.
- Utilizing shot definitions designed to align with human cognition and directorial theories, the goal is to leverage the capabilities of a large language model (LLM) to create a more natural camera timeline by specifying appropriate camera direction based on the scene's context.
- Additionally, it involves composing Shot Sequences and using them to build a MovieRenderQueue pipeline, as well as developing a CLI API to render LevelSequences through a Web API.

##### Topics
- Shot parameter definitions
- AutoCamera, interfacing with LLM
- Implementing shot sequence generation
- Implementing MovieRenderQueue in CLI environment

##### Issues
- Implemention of synchronous(blocked) HTTP request & process with response.
- Motion blur issue when cut change timing in shot sequence.
- Screen snapshot with full lumen illumination applied was required.

---

### Updating MovieScene in UE5
##### Overview
- With the transition from UE4 to UE5, the update mechanism for the SequencePlayer has become almost entirely asynchronous.
- Due to this, the ForceEvaluate, which was frequently used when computations needed to occur according to specific timeframes in the timeline, no longer performs the intended function (updating the scene). As a result, there was a need to find a solution for updating scenes in real projects.
- During this process, a positive side effect was the removal of the SetPlayPosition function, which had been habitually overused in the existing code.

##### Topics
- Interrogator and constraint

##### Issues
- The finalized animation update timing


---
### Others, misc.
- [Domain Setting Guide](https://github.com/dcode1119/DomainSettingGuide) - This page shows how to connect your domain to your github page(README.md)
- [WaveFunc](https://github.com/dcode1119/WaveFunc) - WaveExec.cpp shows how to generate a PCM wave format file.
