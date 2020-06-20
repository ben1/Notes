Begin() requires End() to be called regardless of whether Begin returns false.

Right align an item using:  
```
ImGui.SameLine(GetWindowWidth() - ButtonWidth - ImGui.GetStyle().ItemSpacing.X);
ImGui.Button("Cancel", new Vector2(ButtonWidth, 0));
```

Set keyboard focus only when a window is newly focused (ideally each window would remember keyboard focus, but that doesn't seem to work). 
```
if (ImGui.IsWindowFocused(ImGuiFocusedFlags.RootAndChildWindows) && !ImGui.IsAnyItemActive())  
{  
    ImGui.SetKeyboardFocusHere(0);  
}
```

