# 🚀 nvim-aider

🤖 Seamlessly integrate Aider with Neovim for an enhanced AI-assisted coding experience!

## 🌟 Planned Features

- [x] 🖥️ Aider terminal integration within Neovim
- [x] 🎨 Color theme configuration support
- [ ] 📤 Send buffers, selections, or file names to Aider

## 🎮 Commands

- ⌨️ `AiderTerminalToggle` - Toggle the Aider terminal window
- 📤 `AiderTerminalSend [text]` - Send text to Aider
  - Without arguments: Opens input prompt
  - With arguments: Sends provided text directly

## 🔗 Dependencies

🐍 Python: Install aider  
🌙 Lua: folke/snacks.nvim

## 📦 Installation

Using lazy.nvim:

```lua
{
    "GeorgesAlkhouri/nvim-aider",
    cmd = {
      "AiderTerminalToggle",
    },
    keys = {
      { "<leader>z", "<cmd>AiderTerminalToggle<cr>", desc = "Open Aider" },
    },
    dependencies = {
      "folke/snacks.nvim",
    },
    config = true,
  }
```
