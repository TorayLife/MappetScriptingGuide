---
title: Константы
weight: -80
---

<p align="right">Автор: llama_orp</p>

В MappetExtras вы можете использовать константы! Константы - это неизменные значения, которые в нашем случае будут содержать полезную информацию для методов.

# ***Первый пример:***
```js
function main(c){
    c.player.swingArm(0); // MAIN
    c.player.swingArm(1); // OFF
}
```
Здесь в комментариях приходится пояснять числовые значения.

## Лучше так:
```js
function main(c) {
    const constants = mappet.getConstants();

    c.player.swingArm(constants.MAIN); 
    c.player.swingArm(constants.OFF);
}
```

Теперь мы вызываем именованные константы вместо "магических" чисел. Это позволяет:
* Избавиться от лишних комментариев
* Повысить читабельность кода
* Не запоминать числовые значения

# ***Второй пример:***
```js
function main(c) {
    c.player.setSetting(mappet.getConstants().ATTACK, 0);
}
```
Здесь константа ATTACK возвращает строку "keyBindAttack", которую мы передаем в метод.

Таким образом, константы упрощают работу с методами и делают код более понятным.

# **_Список всех констант:_**
{{< hint type=note >}}
- MAIN - 0;
- OFF - 1;
- ADVANCEMENTS - keyBindAdvancements;
- ATTACK - keyBindAttack;
- BACK - keyBindBack;
- CHAT - keyBindChat;
- COMMAND - keyBindCommand;
- DROP - keyBindDrop;
- FORWARD - keyBindForward;
- FULLSCREEN - keyBindFullscreen;
- INVENTORY - keyBindInventory;
- JUMP - keyBindJump;
- LEFT - keyBindLeft;
- LOAD_TOOLBAR - keyBindLoadToolbar;
- PICK_BLOCK - keyBindPickBlock;
- PLAYER_LIST - keyBindPlayerList;
- RIGHT - keyBindRight;
- SAVE_TOOLBAR - keyBindSaveToolbar;
- SCREENSHOT - keyBindScreenshot;
- HOTBAR - keyBindsHotbar;
- SMOOTH_CAMERA - keyBindSmoothCamera;
- SNEAK - keyBindSneak;
- SPECTATOR_OUTLINES - keyBindSpectatorOutlines;
- SPRINT - keyBindSprint;
- SWAP_HANDS - keyBindSwapHands;
- PERSPECTIVE - keyBindTogglePerspective;
- USE_ITEM - keyBindUseItem;
- PERSON_VIEW - thirdPersonView;
- ITEM_TOOLTIPS - advancedItemTooltips;
- AMBIENT_OCCLUSION - ambientOcclusion;
- ANAGLYPH - anaglyph;
- ATTACK_INDICATOR - attackIndicator;
- AUTO_JUMP - autoJump;
- CHAT_COLOURS - chatColours;
- CHAT_HEIGHT_UNFOCUSED - chatHeightUnfocused;
- CHAT_LINKS - chatLinks;
- CHAT_LINKS_PROMP - chatLinksPromp;
- CHAT_OPACITY - chatOpacity;
- CHAT_SCALE - chatScale;
- CHAT_VISIBLITY - chatVisibility;
- CHAT_WIDTH - chatWidth;
- CLOUDS - clouds;
- DEBUG_CAM - debugCamEnable;
- DIFFICULTY - difficulty;
- VSYNC - enableVsync;
- WEAK_ATTACKS - enableWeakAttacks;
- ENTITY_SHADOWS - entityShadows;
- FANCY_GRAPHICS - fancyGraphics;
- FBO - fboEnable;
- FORCE_UNICODE_FONT - forceUnicodeFont;
- FOV - fovSetting;
- FULL_SCREEN - fullScreen;
- GAMMA - gammaSetting;
- GUI_SCALE - guiScale;
- HELD_ITEM_TOOLTIPS - heldItemTooltips;
- HIDE_GUI - hideGUI;
- HIDE_SERVER_ADDRESS - hideServerAddress;
- INCOMPATIBLE_RESOURCE_PACKS - incompatibleResourcePacks;
- INVERT_MOUSE - invertMouse;
- LANGUAGE - language;
- LAST_SERVER - lastServer;
- LIMIT_FRAMERATE - limitFramerate;
- MAIN_HAND - mainHand;
- MIPMAP_LEVELS - mipmapLevels;
- MOUSE_SENSITIVITY - mouseSensitivity;
- NARRATOR - narrator;
- OVERRIDE_HEIGHT - overrideHeight;
- OVERRIDE_WIDTH - overrideWidth;
- PARTICLE - particleSetting;
- PAUSE_ON_LOST_FOCUS - pauseOnLostFocus;
- REALMS - realmsNotifications;
- REDUCES_DEBUG_INFO - reducedDebugInfo;
- RENDER_DISTANCE_CHUNKS - renderDistanceChunks;
- RESOURCE_PACKS - resourcePacks;
- SATURATION - saturation;
- DEBUG_INFO - showDebugInfo;
- DEBUG_PROFILER_CHART - showDebugProfilerChart;
- LAGOMETER - showLagometer;
- SUBTITLES - showSubtitles;
- CAMERA - smoothCamera;
- SNOOPER - snooperEnabled;
- TOUCH_SCREEN - touchscreen;
- TUTORIAL_STEP - tutorialStep;
- USE_NATIVE_TRANSPORT - useNativeTransport;
- USE_VBO - useVbo;
- VIEW_BOBBING - viewBobbing;
{{< /hint >}}