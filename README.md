# react-html-ai-tag

This repo is for creating an AI based react HTML component

> The following design is based on OpenAI models, we would see if we can adopt more AI models

1. A simple content placement AI component

    ```
    <AI model="model-name" prompt="hello world" type="text/image/audio/video"/>
    ```
    
    Some times we want to store the result or limit the number of content AI will generaate 
    
    ```
    <AI model="model-name" prompt="hello" type="text" store="supabase" frequency="3600"/>
    ```
    
    check by certain logic
    
    ```
    {condition ? <AI model="model-name" prompt="hello" type="text" store="supabase" frequency="3600"/> : null}
    ```

2. Interactive AI component

    ```
    <AI model="model-name" prompt="prompt content" variant="chat" />
    <AI model="model-name" prompt="prompt content" variant="voice" />
    ```
    
    but AI has sensor, we might need add device support
    
    ```
    <AI model="model-name" prompt="prompt content" id="session-id" variant="voice" sensor="none" />
    <AI model="model-name" prompt="prompt content" id="session-id" variant="voice" sensor="all" />
    <AI model="model-name" prompt="prompt content" id="session-id" variant="voice" sensor="camera"/>
    <AI model="model-name" prompt="prompt content" id="session-id" variant="voice" sensor="temperature"/>
    <AI model="model-name" prompt="prompt content" id="session-id" variant="voice" sensor="touch"/>
    <AI model="model-name" prompt="prompt content" id="session-id" variant="voice" sensor="sensor-id"/>
    <AI model="model-name" prompt="prompt content" id="session-id" variant="voice" sensor="[sensor-id1,sensor-id2]"/>
    ```


