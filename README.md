# One Dark Theme
A Home Assistant theme inspired by atoms one dark theme and built on the [Google Dark Theme](https://github.com/JuanMTech/google_dark_theme) by JuanMTech.

### Screenshots

**This is work in progress**

**1. Desktop**
<p align="center">
  <!--img src="https://i.imgur.com/CS3N3kB.png"-->
</p>

**2. Mobile**

<p align="center">
  <!--img src="https://i.imgur.com/D4RDkiG.png"-->
</p>

### Preparation
1. Make sure that under the **configuration.yaml** file you have the following:

```yaml
frontend:
  themes: !include_dir_merge_named themes
```

2. Under the Home Assistant **Config** folder, create a new folder named **themes**
3. **Restart** Home assistant to apply the changes. 

### HACS installation
1. Go into the Community Store (HACS)
2. Search for One Dark Theme
3. Open the theme
4. Press Install
5. Restart Home Assistant

### Manual installation
1. In the Home assistant **themes** folder, create a file named `one_dark_theme.yaml`
2. In this GitHub repo, go into the **themes** folder, open the `one_dark_theme.yaml` file and copy the content
3. Paste the content in the `one_dark_theme.yaml` file created under your Home Assistant themes folder

### Enable theme
1. Open your Home Assistant **Profile**
2. Under, **Themes**, select the One Dark Theme


### Custom Header settings
When using the [Custom Header](https://github.com/maykar/custom-header) plugin, add the following to make sure that the header matches the theme.

```yaml
custom_header:
  compact_mode: true
  background: var(--app-header-background-color)
  elements_color: var(--app-header-text-color)
  active_tab_color: var(--state-icon-active-color)
  tab_indicator_color: var(--state-icon-active-color)
```
