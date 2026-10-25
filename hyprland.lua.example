local active_border_color = { colors = { "rgba(9fb0f2ee)", "rgba(f1c4dcee)" }, angle = 45 }
local inactive_border_color = "rgba(ffffff88)"

hl.config({
  general = {
    col = {
      active_border = active_border_color,
      inactive_border = inactive_border_color,
    },
  },

  group = {
    col = {
      border_active = active_border_color,
      border_inactive = inactive_border_color,
    },
  },

  -- Liquid Glass is soft frosted panes: rounded corners, a light lavender
  -- shadow, and a bright blur that keeps the pastel backdrop from going grey.
  decoration = {
    rounding = 14,

    shadow = {
      enabled = true,
      range = 18,
      render_power = 3,
      color = "rgba(7a86c833)",
      color_inactive = "rgba(7a86c41a)",
    },

    blur = {
      enabled = true,
      size = 8,
      passes = 3,
      new_optimizations = true,
      xray = false,
      contrast = 0.9,
      brightness = 1.05,
      noise = 0.01,
      vibrancy = 0.25,
      vibrancy_darkness = 0.0,
      popups = true,
      special = true,
    },
  },
})

-- The shell surfaces are translucent in this theme, so frost what is behind them.
hl.layer_rule({
  match = { namespace = "^(omarchy-bar|omarchy-menu|omarchy-notifications|omarchy-osd|omarchy-polkit|omarchy-reminders|omarchy-clipboard|omarchy-emojis|omarchy-keyboard-panel|omarchy-network-qr)$" },
  blur = true,
  ignore_alpha = 0.3,
})
