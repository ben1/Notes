Begin() requires End() to be called regardless of whether Begin returns false.
Right align an item using:
  SameLine(GetWindowWidth() - ButtonWidth - ImGui::GetStyle().ItemSpacing.x);
  ImGui.Button("Cancel", ImVec2(ButtonWidth, 0));

