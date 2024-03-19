# DMX TOOLS

# Components

## Light Components

### DMX_LightColorComponent

Add this component to any light actor in the scene to enable color control of the light from dmx. Set the Universe and Address of the light in the details panel of the component. The maximum intensity of the light will be the brightness value listed in the details panel.

All light components parented to this actor will be affected.

Choose either 8 or 16 bit mode. 

Channel list:
| Function    | 8 bit | 16 Bit | 24 bit |
| --------    | ----- | ------ | ------ |
| Red         | 1     | 1      | 1      |
| Red Fine    |       | 2      | 2      |
| Red Ultra   |       |        | 3      |
| Green       | 2     | 3      | 4      |
| Green Fine  |       | 4      | 5      |
| Green Ultra |       |        | 6      |
| Blue        | 3     | 5      | 7      |
| Blue Fine   |       | 6      | 8      |
| Blue Ultra  |       |        | 9      |




### DMX_LightIntensityComponent

Add this component to any light actor in the scene to enable intensity control of the light. Set the Universe and Address in the details panel of the component. The color of the light is still controlled by the individual light component.

All light components parented to this actor will be affected. 

Choose either 8, 16, or 24 bit mode. 

Channel list:

| Function   | 8 bit | 16 bit | 24 bit |
| --------   | ----- | ------ | ------ |
| Dim Coarse | 1     | 1      | 1      |
| Dim Fine   |       | 2      | 2      |
| Dim Ultra  |       |        | 3      |

## Materials

There are two ways to work with dmx controllable materials in this set of tools. The first gives quickly accessible building blocks that allow for quick and simple material creation, the second allows for greater customization.

For simple creation and materials, use the included DMX_Material. You can create an instance of this material to change the diffuse and emission colors, or the metallic, roughness, or specularity. These values can be previewed in the editor, but will be overwritten by whatever dmx values are assigned to them during playback/runtime. 
All the components associated with the included DMX_Material can be used in composition- that is if you want to control just the diffuse color and roughness of a material, you can add just the DMX_MaterialDiffuse and DMX_MaterialRoughness components to that actor. 

Each Material component has a setting for the material index of the actor. The control of the component will target only the material in the specified material slot- this defaults to 0, the first material in any actor. 

Custom dmx controllable materials will be covered in the DMX_MaterialCustom component documentation. 




### DMX_MaterialAll

This component works with the included DMX_Material instance.

This component controls the materials diffuse color, emissive color, metalness, specularity, and roughness in a single component.

Set the universe and address of the material in the details panel of the component. 

Channel List:

| Function             | 8 bit | 16 Bit | 24 bit |
| --------             | ----- | ------ | ------ |
| Diffuse Red          | 1     | 1      | 1      |
| Diffuse Red Fine     |       | 2      | 2      |
| Diffuse Red Ultra    |       |        | 3      |
| Diffuse Green        | 2     | 3      | 4      |
| Diffuse Green Fine   |       | 4      | 5      |
| Diffuse Green Ultra  |       |        | 6      |
| Diffuse Blue         | 3     | 5      | 7      |
| Diffuse Blue Fine    |       | 6      | 8      |
| Diffuse Blue Ultra   |       |        | 9      |
| Emissive Red         | 4     | 7      | 10     |
| Emissive Red Fine    |       | 8      | 11     |
| Emissive Red Ultra   |       |        | 12     |
| Emissive Green       | 5     | 9      | 13     |
| Emissive Green Fine  |       | 10     | 14     |
| Emissive Green Ultra |       |        | 15     |
| Emissive Blue        | 6     | 11     | 16     |
| Emissive Blue Fine   |       | 12     | 17     |
| Emissive Blue Ultra  |       |        | 18     |
| Metallic             | 7     | 13     | 19     |
| Metallic Fine        |       | 14     | 20     |
| Metallic Ultra       |       |        | 21     |
| Specular             | 8     | 15     | 22     | 
| Speclar Fine         |       | 16     | 23     |
| Specular Ultra       |       |        | 24     |
| Roughness            | 9     | 17     | 25     |
| Roughness Fine       |       | 18     | 26     |
| Roughness Ultra      |       |        | 27     |




### DMX_MaterialDiffuse

This component works with the included DMX_Material instance.

This component controls the materials diffuse color only. 

Set the universe and address of the material in the details panel of the component. 


Channel List:

| Function             | 8 bit | 16 Bit | 24 bit |
| --------             | ----- | ------ | ------ |
| Diffuse Red          | 1     | 1      | 1      |
| Diffuse Red Fine     |       | 2      | 2      |
| Diffuse Red Ultra    |       |        | 3      |
| Diffuse Green        | 2     | 3      | 4      |
| Diffuse Green Fine   |       | 4      | 5      |
| Diffuse Green Ultra  |       |        | 6      |
| Diffuse Blue         | 3     | 5      | 7      |
| Diffuse Blue Fine    |       | 6      | 8      |
| Diffuse Blue Ultra   |       |        | 9      |

### DMX_MaterialEmissive

This component works with the included DMX_Material instance.

This component controls the materials emissive color only. 

Set the universe and address of the material in the details panel of the component. 


Channel List:

| Function             | 8 bit | 16 Bit | 24 bit |
| --------             | ----- | ------ | ------ |
| Emissive Red          | 1     | 1      | 1      |
| Emissive Red Fine     |       | 2      | 2      |
| Emissive Red Ultra    |       |        | 3      |
| Emissive Green        | 2     | 3      | 4      |
| Emissive Green Fine   |       | 4      | 5      |
| Emissive Green Ultra  |       |        | 6      |
| Emissive Blue         | 3     | 5      | 7      |
| Emissive Blue Fine    |       | 6      | 8      |
| Emissive Blue Ultra   |       |        | 9      |


### DMX_MaterialMetallic

This component works with the included DMX_Material instance.

This component controls the materials metalness only.

Set the Universe and Address of the material in the details panel of the component. 

Channel List:

| Function             | 8 bit | 16 bit | 24 bit |
| -------------------- | ----- | ------ | ------ |
| Metallic             | 1     | 1      | 1      |
| Metallic Fine        |       | 2      | 2      |
| Metallic Ultra       |       |        | 3      |


### DMX_MaterialSpecular

This component works with the included DMX_Material instance.

This component controls the materials specularity only.

Set the Universe and Address of the material in the details panel of the component. 

Channel List:

| Function             | 8 bit | 16 bit | 24 bit |
| -------------------- | ----- | ------ | ------ |
| Specular             | 1     | 1      | 1      |
| Specular Fine        |       | 2      | 2      |
| Specular Ultra       |       |        | 3      |


### DMX_MaterialRoughness

This component works with the included DMX_Material instance.

This component controls the materials roughness only.

Set the Universe and Address of the material in the details panel of the component. 

Channel List:

| Function              | 8 bit | 16 bit | 24 bit |
| --------------------- | ----- | ------ | ------ |
| Roughness             | 1     | 1      | 1      |
| Roughness Fine        |       | 2      | 2      |
| Roughness Ultra       |       |        | 3      |


### DMX_MaterialCustom

Use this material to use custom parameters in materials you create yourself. You can use this to define your own custom parameters that will be dmx controllable in your material instances.
Apply this component and your material to your actor. In the details panel of the component, add an element to the "Material Parameters" attribute. Give your parameter a name, and select if you would like it to be a color or float value, and if it will be an 8 bit or 16 bit dmx channel. 

In the material editor, add a constant to the graph editor. If you chose a color value, use a constant3vector. If you chose a float value, use a single constant. Right click the node and convert it to a parameter, and give it the same name you did in the component detail panel. 

The parameters in your material will then be controllable via dmx in actors with the DMX_MaterialCustom component. Float values will be acessible in the material graph editor mapped in a range from 0 to 1. 

The dmx address of each material parameter used will increment by the number of channels it takes up, in the same order they are listed in the Material Parameters in the component details panel. 

For example, if you have a material with 3 parameters- Base Color (16 bit Color), Normal Strength (16 bit float), and Overlay Color (8 bit Color) - and patch it starting at address 1,  the corresponding dmx addresses for each parameter would be: Base color- address 1, Normal strength - address 7, and Overlay Color - address 9. The whole material would have a Dmx footprint of 11 channels. 

Since using this component is highly customizable, it's left to the user to create an appropriate fixture profile in their lighting console. 


## Triggers

### DMX_TriggerComponent

This component is used to trigger events in the blueprint of the parent actor. It exposes 2 events in the parent actor's event graph- Event On Dmx Activated, and Event On Dmx Deactivated. 
The Event On Dmx Activated is fired once after the Dmx value goes above the specified threshold value, and Event On Dmx Deactivated is fired once after the Dmx value goes below that threshold value again. The component must become activated before it can fire the deactivated event.

Set the desired Universe and Address in the details panel of the component. 
The Threshold value in the details panel sets the value at which the component will trigger the activated and deactivated events. It can be a range from 0 to 254. 

In order to use this component, the parent actor you want to control must implement the DMX_TriggerInterface blueprint interface. To set this on the parent actor, go to its blueprint class settings, and add this interface in the class settings details panel. After it's been added to the interface list, the On Dmx Activate and On Dmx Deactivate events will be available in the blueprint actor's event graph. 

The Dmx trigger uses a single 8 bit Dmx channel. 