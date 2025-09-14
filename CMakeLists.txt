if ((NOT CONFIG_ZMK_SPLIT) OR CONFIG_ZMK_SPLIT_ROLE_CENTRAL)
  target_sources_ifdef(CONFIG_ZMK_BEHAVIOR_CAPS_WORD_DE app PRIVATE src/behaviors/behavior_caps_word_de.c)

  zephyr_include_directories(include)
endif()
