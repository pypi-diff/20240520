# Comparing `tmp/rio_ui-0.7.1.tar.gz` & `tmp/rio_ui-0.7.2.tar.gz`

## Comparing `rio_ui-0.7.1.tar` & `rio_ui-0.7.2.tar`

### file list

```diff
@@ -1,365 +1,365 @@
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 rio_ui-0.7.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 rio_ui-0.7.1/.prettierrc
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 rio_ui-0.7.1/.sassrc
--rw-r--r--   0        0        0     5534 2020-02-02 00:00:00.000000 rio_ui-0.7.1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 rio_ui-0.7.1/CONTRIBUTING.md
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 rio_ui-0.7.1/changelog.md
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 rio_ui-0.7.1/package.json
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 rio_ui-0.7.1/vite.config.js
--rw-r--r--   0        0        0     5140 2020-02-02 00:00:00.000000 rio_ui-0.7.1/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/index.html
--rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/app.ts
--rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/colorConversion.ts
--rw-r--r--   0        0        0    20706 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/componentManagement.ts
--rw-r--r--   0        0        0     5795 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/cssUtils.ts
--rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/dataModels.ts
--rw-r--r--   0        0        0     6925 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/designApplication.ts
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/easeFunctions.ts
--rw-r--r--   0        0        0     4869 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/eventHandling.ts
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/inputBoxTools.ts
--rw-r--r--   0        0        0     6081 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/layoutHelpers.ts
--rw-r--r--   0        0        0     4878 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/layouting.ts
--rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/rippleEffect.ts
--rw-r--r--   0        0        0    11646 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/rpc.ts
--rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/rpcFunctions.ts
--rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/utils.ts
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/components/align.ts
--rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/components/buildFailed.ts
--rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/components/button.ts
--rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/components/card.ts
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/components/classContainer.ts
--rw-r--r--   0        0        0     6349 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/components/codeBlock.ts
--rw-r--r--   0        0        0    15146 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/components/codeExplorer.ts
--rw-r--r--   0        0        0    13820 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/components/colorPicker.ts
--rw-r--r--   0        0        0    13570 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/components/componentBase.ts
--rw-r--r--   0        0        0    14334 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/components/componentTree.ts
--rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/components/customListItem.ts
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/components/debuggerConnector.ts
--rw-r--r--   0        0        0    11400 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/components/drawer.ts
--rw-r--r--   0        0        0    16927 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/components/dropdown.ts
--rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/components/flowContainer.ts
--rw-r--r--   0        0        0     5700 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/components/fundamentalRootComponent.ts
--rw-r--r--   0        0        0    11004 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/components/grid.ts
--rw-r--r--   0        0        0     2201 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/components/headingListItem.ts
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/components/html.ts
--rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/components/icon.ts
--rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/components/image.ts
--rw-r--r--   0        0        0    19839 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/components/keyEventListener.ts
--rw-r--r--   0        0        0     9923 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/components/linearContainers.ts
--rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/components/link.ts
--rw-r--r--   0        0        0     4575 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/components/listView.ts
--rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/components/margin.ts
--rw-r--r--   0        0        0     6268 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/components/markdown.ts
--rw-r--r--   0        0        0    27995 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/components/mediaPlayer.ts
--rw-r--r--   0        0        0     5948 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/components/mouseEventListener.ts
--rw-r--r--   0        0        0     4122 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/components/multiLineTextInput.ts
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/components/nodeInput.ts
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/components/nodeOutput.ts
--rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/components/overlay.ts
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/components/placeholder.ts
--rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/components/plot.ts
--rw-r--r--   0        0        0     7055 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/components/popup.ts
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/components/progressBar.ts
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/components/progressCircle.ts
--rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/components/rectangle.ts
--rw-r--r--   0        0        0    10840 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/components/revealer.ts
--rw-r--r--   0        0        0     9454 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/components/scrollContainer.ts
--rw-r--r--   0        0        0     6620 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/components/scrollTarget.ts
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/components/separator.ts
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/components/separatorListItem.ts
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/components/singleContainer.ts
--rw-r--r--   0        0        0     5031 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/components/slider.ts
--rw-r--r--   0        0        0     7104 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/components/slideshow.ts
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/components/stack.ts
--rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/components/switch.ts
--rw-r--r--   0        0        0     8056 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/components/switcher.ts
--rw-r--r--   0        0        0    19999 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/components/switcherBar.ts
--rw-r--r--   0        0        0     8067 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/components/table.ts
--rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/components/text.ts
--rw-r--r--   0        0        0     7311 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/components/textInput.ts
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/components/themeContextSwitcher.ts
--rw-r--r--   0        0        0     4463 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/components/tooltip.ts
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/code/components/website.ts
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/css/highlightjs-default-dark.css
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/css/highlightjs-default-light.css
--rw-r--r--   0        0        0    50930 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/css/style.scss
--rw-r--r--   0        0        0     8244 2020-02-02 00:00:00.000000 rio_ui-0.7.1/frontend/css/switcheroos.scss
--rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 rio_ui-0.7.1/raw-icons/custom-material-icons/twinkle.svg
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 rio_ui-0.7.1/raw-icons/custom-material-icons/fill/twinkle.svg
--rw-r--r--   0        0        0    10067 2020-02-02 00:00:00.000000 rio_ui-0.7.1/raw-icons/rio/logo-and-text-horizontal.svg
--rw-r--r--   0        0        0    10127 2020-02-02 00:00:00.000000 rio_ui-0.7.1/raw-icons/rio/logo-and-text-vertical.svg
--rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 rio_ui-0.7.1/raw-icons/rio/logo.svg
--rw-r--r--   0        0        0     5933 2020-02-02 00:00:00.000000 rio_ui-0.7.1/raw-icons/rio/color/logo-and-text-horizontal.svg
--rw-r--r--   0        0        0     5961 2020-02-02 00:00:00.000000 rio_ui-0.7.1/raw-icons/rio/color/logo-and-text-vertical.svg
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 rio_ui-0.7.1/raw-icons/rio/color/logo.svg
--rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 rio_ui-0.7.1/raw-icons/rio/fill/logo-and-text-horizontal.svg
--rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 rio_ui-0.7.1/raw-icons/rio/fill/logo-and-text-vertical.svg
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 rio_ui-0.7.1/raw-icons/rio/fill/logo.svg
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 rio_ui-0.7.1/raw-icons/styling/corner-round-bottom-left.svg
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 rio_ui-0.7.1/raw-icons/styling/corner-round-bottom-right.svg
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 rio_ui-0.7.1/raw-icons/styling/corner-round-top-left.svg
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 rio_ui-0.7.1/raw-icons/styling/corner-round-top-right.svg
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/__init__.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/__main__.py
--rw-r--r--   0        0        0    19320 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/app.py
--rw-r--r--   0        0        0    32919 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/app_server.py
--rw-r--r--   0        0        0     8672 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/assets.py
--rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/byte_serving.py
--rw-r--r--   0        0        0    19465 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/color.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/cursor_style.py
--rw-r--r--   0        0        0     6033 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/dataclass.py
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/errors.py
--rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/event.py
--rw-r--r--   0        0        0     6690 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/fills.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/global_state.py
--rw-r--r--   0        0        0     9857 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/icon_registry.py
--rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/inspection.py
--rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/maybes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/py.typed
--rw-r--r--   0        0        0     8057 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/routing.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/self_serializing.py
--rw-r--r--   0        0        0     8519 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/serialization.py
--rw-r--r--   0        0        0    79752 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/session.py
--rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/session_attachments.py
--rw-r--r--   0        0        0     8246 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/state_properties.py
--rw-r--r--   0        0        0     4492 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/text_style.py
--rw-r--r--   0        0        0    28614 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/theme.py
--rw-r--r--   0        0        0     5401 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/user_settings_module.py
--rw-r--r--   0        0        0    10026 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/utils.py
--rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/world_units.py
--rw-r--r--   0        0        0    11560 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/assets/fonts/Roboto/LICENSE.txt
--rw-r--r--   0        0        0   167336 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/assets/fonts/Roboto/Roboto-Bold.ttf
--rw-r--r--   0        0        0   171508 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/assets/fonts/Roboto/Roboto-BoldItalic.ttf
--rw-r--r--   0        0        0   170504 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/assets/fonts/Roboto/Roboto-Italic.ttf
--rw-r--r--   0        0        0   168260 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/assets/fonts/Roboto/Roboto-Regular.ttf
--rw-r--r--   0        0        0    11560 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/assets/fonts/Roboto Mono/LICENSE.txt
--rw-r--r--   0        0        0    87392 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/assets/fonts/Roboto Mono/RobotoMono-Bold.ttf
--rw-r--r--   0        0        0    94636 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/assets/fonts/Roboto Mono/RobotoMono-BoldItalic.ttf
--rw-r--r--   0        0        0    94372 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/assets/fonts/Roboto Mono/RobotoMono-Italic.ttf
--rw-r--r--   0        0        0    87236 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/assets/fonts/Roboto Mono/RobotoMono-Regular.ttf
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/assets/hosted/README.md
--rw-r--r--   0        0        0    54189 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/assets/hosted/rio-logos/logo-and-text-horizontal.png
--rw-r--r--   0        0        0    31665 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/assets/hosted/rio-logos/rio-logo-square.png
--rw-r--r--   0        0        0  1081336 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/assets/icon-sets/material.tar.xz
--rw-r--r--   0        0        0    14992 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/assets/icon-sets/rio.tar.xz
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/assets/icon-sets/styling.tar.xz
--rw-r--r--   0        0        0     7375 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/cli/__init__.py
--rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/cli/cli_instance.py
--rw-r--r--   0        0        0     6672 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/cli/nice_traceback.py
--rw-r--r--   0        0        0    14016 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/cli/project.py
--rw-r--r--   0        0        0    14492 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/cli/project_setup.py
--rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/cli/rio_api.py
--rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/cli/rioignore.py
--rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/cli/tomlconfig.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/cli/run_project/__init__.py
--rw-r--r--   0        0        0     5446 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/cli/run_project/app_loading.py
--rw-r--r--   0        0        0    22577 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/cli/run_project/arbiter.py
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/cli/run_project/file_watcher_worker.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/cli/run_project/run_models.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/cli/run_project/run_utils.py
--rw-r--r--   0        0        0     4155 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/cli/run_project/uvicorn_worker.py
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/cli/run_project/webview_worker.py
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/__init__.py
--rw-r--r--   0        0        0     4469 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/app_root.py
--rw-r--r--   0        0        0     4167 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/auto_form.py
--rw-r--r--   0        0        0     4800 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/banner.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/build_failed.py
--rw-r--r--   0        0        0    12739 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/button.py
--rw-r--r--   0        0        0     5325 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/card.py
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/class_container.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/code_block.py
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/code_explorer.py
--rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/color_picker.py
--rw-r--r--   0        0        0    26340 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/component.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/component_tree.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/container.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/debugger_connector.py
--rw-r--r--   0        0        0     4152 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/devel_component.py
--rw-r--r--   0        0        0     4274 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/drawer.py
--rw-r--r--   0        0        0     7070 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/dropdown.py
--rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/flow_container.py
--rw-r--r--   0        0        0     6075 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/fundamental_component.py
--rw-r--r--   0        0        0     7087 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/grid.py
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/html.py
--rw-r--r--   0        0        0     7709 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/icon.py
--rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/image.py
--rw-r--r--   0        0        0    14169 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/key_event_listener.py
--rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/labeled_column.py
--rw-r--r--   0        0        0    10697 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/linear_containers.py
--rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/link.py
--rw-r--r--   0        0        0    10524 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/list_items.py
--rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/list_view.py
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/markdown.py
--rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/media_player.py
--rw-r--r--   0        0        0    10800 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/mouse_event_listener.py
--rw-r--r--   0        0        0     5140 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/multi_line_text_input.py
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/node_input.py
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/node_output.py
--rw-r--r--   0        0        0     9335 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/number_input.py
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/overlay.py
--rw-r--r--   0        0        0     5147 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/page_view.py
--rw-r--r--   0        0        0     4992 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/plot.py
--rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/popup.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/progress_bar.py
--rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/progress_circle.py
--rw-r--r--   0        0        0     5702 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/rectangle.py
--rw-r--r--   0        0        0     4038 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/revealer.py
--rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/root_components.py
--rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/scroll_container.py
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/scroll_target.py
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/separator.py
--rw-r--r--   0        0        0     5947 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/slider.py
--rw-r--r--   0        0        0     3585 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/slideshow.py
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/spacer.py
--rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/stack.py
--rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/switch.py
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/switcher.py
--rw-r--r--   0        0        0     9204 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/switcher_bar.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/table.py
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/text.py
--rw-r--r--   0        0        0     6144 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/text_input.py
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/theme_context_switcher.py
--rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/tooltip.py
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/components/website.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/debug/__init__.py
--rw-r--r--   0        0        0     7485 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/debug/monkeypatches.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/debug/typing_utils.py
--rw-r--r--   0        0        0    14479 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/debug/validator.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/debug/dev_tools/__init__.py
--rw-r--r--   0        0        0    10582 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/debug/dev_tools/component_details.py
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/debug/dev_tools/deploy_page.py
--rw-r--r--   0        0        0     3598 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/debug/dev_tools/dev_tools_sidebar.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/debug/dev_tools/docs_page.py
--rw-r--r--   0        0        0    12890 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/debug/dev_tools/icons_page.py
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/debug/dev_tools/layout_preview.py
--rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/debug/dev_tools/project_page.py
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/debug/dev_tools/sample_icons_grid.py
--rw-r--r--   0        0        0    17346 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/debug/dev_tools/theme_picker_page.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/debug/dev_tools/tree_page.py
--rw-r--r--   0        0        0    10466 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/docs/__init__.py
--rw-r--r--   0        0        0   416487 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/generated/index.html
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/patches_for_3rd_party_stuff/IocpProactor_accept_locals_accept_coro.py
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/patches_for_3rd_party_stuff/ProactorBasePipeTransport_call_connection_lost.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/patches_for_3rd_party_stuff/_OverlappedFuture_cancel_overlapped.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/patches_for_3rd_party_stuff/__init__.py
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/README.md
--rw-r--r--   0        0        0    15602 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/__init__.py
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/howtos/core-classes.md
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/howtos/debugging-setup.md
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/howtos/deployment.md
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/howtos/howto-custom-events.md
--rw-r--r--   0        0        0     5844 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/howtos/howto-get-value-from-child-component.md
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/howtos/howto-install.md
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/howtos/howto-pass-value-to-event.md
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/howtos/persistent-settings.md
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/howtos/project-setup.md
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/howtos/run-project.md
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/howtos/theming.md
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/howtos-todo/attribute-bindings.md
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/howtos-todo/component-lifecycle.md
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/howtos-todo/custom-events.md
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/howtos-todo/force-refresh.md
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/howtos-todo/initialize-component-asynchronously.md
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/howtos-todo/layouting.md
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/howtos-todo/multiple-pages.md
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/other-examples/simple_counter_app.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-AI Chatbot/README.md
--rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-AI Chatbot/conversation.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-AI Chatbot/meta.json
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-AI Chatbot/root_init.py
--rw-r--r--   0        0        0   258496 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-AI Chatbot/thumbnail.svg
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-AI Chatbot/components/__init__.py
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_message.py
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_suggestion_card.py
--rw-r--r--   0        0        0     3728 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-AI Chatbot/components/empty_chat_placeholder.py
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-AI Chatbot/components/generating_response_placeholder.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-AI Chatbot/pages/__init__.py
--rw-r--r--   0        0        0     5823 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-AI Chatbot/pages/chat_page.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Crypto Dashboard/README.md
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Crypto Dashboard/data_models.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Crypto Dashboard/meta.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Crypto Dashboard/root_init.py
--rw-r--r--   0        0        0   270445 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Crypto Dashboard/thumbnail.svg
--rw-r--r--   0        0        0     7595 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Crypto Dashboard/assets/cryptos.csv
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/__init__.py
--rw-r--r--   0        0        0    10704 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/balance_card.py
--rw-r--r--   0        0        0     6695 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_card.py
--rw-r--r--   0        0        0     5604 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_chart.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Crypto Dashboard/pages/__init__.py
--rw-r--r--   0        0        0     7668 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Crypto Dashboard/pages/dashboard_page.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Empty/README.md
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Empty/meta.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Empty/root_init.py
--rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Empty/thumbnail.svg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Empty/pages/__init__.py
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Empty/pages/sample_page.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Multipage Website/README.md
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Multipage Website/meta.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Multipage Website/root_init.py
--rw-r--r--   0        0        0   208005 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Multipage Website/thumbnail.svg
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Multipage Website/components/__init__.py
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Multipage Website/components/footer.py
--rw-r--r--   0        0        0     4826 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Multipage Website/components/navbar.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Multipage Website/components/news_article.py
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Multipage Website/components/testimonial.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Multipage Website/pages/__init__.py
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Multipage Website/pages/about_page.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Multipage Website/pages/home_page.py
--rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Multipage Website/pages/news_page.py
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Multipage Website/pages/root_page.py
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Simple CRUD/README.md
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Simple CRUD/data_models.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Simple CRUD/meta.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Simple CRUD/root_init.py
--rw-r--r--   0        0        0   350009 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Simple CRUD/thumbnail.svg
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Simple CRUD/components/__init__.py
--rw-r--r--   0        0        0     7284 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_editor.py
--rw-r--r--   0        0        0     5810 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_list.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Simple CRUD/pages/__init__.py
--rw-r--r--   0        0        0     8587 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Simple CRUD/pages/crud_page.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/README.md
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/meta.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/root_init.py
--rw-r--r--   0        0        0    23769 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/thumbnail.svg
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/__init__.py
--rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/field.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/__init__.py
--rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/tic_tac_toe_page.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/components/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/__init__.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/tic_tac_toe_page.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/__init__.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/field.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/__init__.py
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/tic_tac_toe_page.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/__init__.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/field.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/__init__.py
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/tic_tac_toe_page.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/__init__.py
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/field.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/__init__.py
--rw-r--r--   0        0        0     4348 2020-02-02 00:00:00.000000 rio_ui-0.7.1/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/tic_tac_toe_page.py
--rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 rio_ui-0.7.1/scripts/benchmark.py
--rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 rio_ui-0.7.1/scripts/build_material_icon_set.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 rio_ui-0.7.1/scripts/cloc.sh
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 rio_ui-0.7.1/scripts/code_coverage.py
--rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 rio_ui-0.7.1/scripts/publish_new_release.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 rio_ui-0.7.1/tests/test_app_build.py
--rw-r--r--   0        0        0     8822 2020-02-02 00:00:00.000000 rio_ui-0.7.1/tests/test_attribute_bindings.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 rio_ui-0.7.1/tests/test_custom_components.py
--rw-r--r--   0        0        0     3426 2020-02-02 00:00:00.000000 rio_ui-0.7.1/tests/test_docstring_code_blocks.py
--rw-r--r--   0        0        0     3797 2020-02-02 00:00:00.000000 rio_ui-0.7.1/tests/test_documentation.py
--rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 rio_ui-0.7.1/tests/test_events.py
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 rio_ui-0.7.1/tests/test_project_templates.py
--rw-r--r--   0        0        0    11737 2020-02-02 00:00:00.000000 rio_ui-0.7.1/tests/test_reconciliation.py
--rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 rio_ui-0.7.1/tests/test_refresh.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 rio_ui-0.7.1/tests/test_session.py
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 rio_ui-0.7.1/tests/test_user_settings.py
--rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 rio_ui-0.7.1/tests/test_zzz_guardrails.py
--rw-r--r--   0        0        0     8596 2020-02-02 00:00:00.000000 rio_ui-0.7.1/tests/utils.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 rio_ui-0.7.1/.gitignore
--rw-r--r--   0        0        0    11315 2020-02-02 00:00:00.000000 rio_ui-0.7.1/LICENSE.txt
--rw-r--r--   0        0        0     7523 2020-02-02 00:00:00.000000 rio_ui-0.7.1/README.md
--rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 rio_ui-0.7.1/pyproject.toml
--rw-r--r--   0        0        0    22744 2020-02-02 00:00:00.000000 rio_ui-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 rio_ui-0.7.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 rio_ui-0.7.2/.prettierrc
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 rio_ui-0.7.2/.sassrc
+-rw-r--r--   0        0        0     5534 2020-02-02 00:00:00.000000 rio_ui-0.7.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 rio_ui-0.7.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 rio_ui-0.7.2/changelog.md
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 rio_ui-0.7.2/package.json
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 rio_ui-0.7.2/vite.config.js
+-rw-r--r--   0        0        0     5140 2020-02-02 00:00:00.000000 rio_ui-0.7.2/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/index.html
+-rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/app.ts
+-rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/colorConversion.ts
+-rw-r--r--   0        0        0    20706 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/componentManagement.ts
+-rw-r--r--   0        0        0     5795 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/cssUtils.ts
+-rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/dataModels.ts
+-rw-r--r--   0        0        0     6925 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/designApplication.ts
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/easeFunctions.ts
+-rw-r--r--   0        0        0     4869 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/eventHandling.ts
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/inputBoxTools.ts
+-rw-r--r--   0        0        0     6081 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/layoutHelpers.ts
+-rw-r--r--   0        0        0     4878 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/layouting.ts
+-rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/rippleEffect.ts
+-rw-r--r--   0        0        0    11646 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/rpc.ts
+-rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/rpcFunctions.ts
+-rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/utils.ts
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/align.ts
+-rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/buildFailed.ts
+-rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/button.ts
+-rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/card.ts
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/classContainer.ts
+-rw-r--r--   0        0        0     6349 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/codeBlock.ts
+-rw-r--r--   0        0        0    15146 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/codeExplorer.ts
+-rw-r--r--   0        0        0    13820 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/colorPicker.ts
+-rw-r--r--   0        0        0    13570 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/componentBase.ts
+-rw-r--r--   0        0        0    14334 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/componentTree.ts
+-rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/customListItem.ts
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/debuggerConnector.ts
+-rw-r--r--   0        0        0    11400 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/drawer.ts
+-rw-r--r--   0        0        0    16927 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/dropdown.ts
+-rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/flowContainer.ts
+-rw-r--r--   0        0        0     5700 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/fundamentalRootComponent.ts
+-rw-r--r--   0        0        0    11004 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/grid.ts
+-rw-r--r--   0        0        0     2201 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/headingListItem.ts
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/html.ts
+-rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/icon.ts
+-rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/image.ts
+-rw-r--r--   0        0        0    19839 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/keyEventListener.ts
+-rw-r--r--   0        0        0     9923 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/linearContainers.ts
+-rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/link.ts
+-rw-r--r--   0        0        0     4575 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/listView.ts
+-rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/margin.ts
+-rw-r--r--   0        0        0     6268 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/markdown.ts
+-rw-r--r--   0        0        0    27995 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/mediaPlayer.ts
+-rw-r--r--   0        0        0     5948 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/mouseEventListener.ts
+-rw-r--r--   0        0        0     4122 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/multiLineTextInput.ts
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/nodeInput.ts
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/nodeOutput.ts
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/overlay.ts
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/placeholder.ts
+-rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/plot.ts
+-rw-r--r--   0        0        0     7055 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/popup.ts
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/progressBar.ts
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/progressCircle.ts
+-rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/rectangle.ts
+-rw-r--r--   0        0        0    10840 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/revealer.ts
+-rw-r--r--   0        0        0     9454 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/scrollContainer.ts
+-rw-r--r--   0        0        0     6620 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/scrollTarget.ts
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/separator.ts
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/separatorListItem.ts
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/singleContainer.ts
+-rw-r--r--   0        0        0     5031 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/slider.ts
+-rw-r--r--   0        0        0     7104 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/slideshow.ts
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/stack.ts
+-rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/switch.ts
+-rw-r--r--   0        0        0     8056 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/switcher.ts
+-rw-r--r--   0        0        0    19999 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/switcherBar.ts
+-rw-r--r--   0        0        0     8067 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/table.ts
+-rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/text.ts
+-rw-r--r--   0        0        0     7311 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/textInput.ts
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/themeContextSwitcher.ts
+-rw-r--r--   0        0        0     4463 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/tooltip.ts
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/website.ts
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/css/highlightjs-default-dark.css
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/css/highlightjs-default-light.css
+-rw-r--r--   0        0        0    50930 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/css/style.scss
+-rw-r--r--   0        0        0     8244 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/css/switcheroos.scss
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 rio_ui-0.7.2/raw-icons/custom-material-icons/twinkle.svg
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 rio_ui-0.7.2/raw-icons/custom-material-icons/fill/twinkle.svg
+-rw-r--r--   0        0        0    10067 2020-02-02 00:00:00.000000 rio_ui-0.7.2/raw-icons/rio/logo-and-text-horizontal.svg
+-rw-r--r--   0        0        0    10127 2020-02-02 00:00:00.000000 rio_ui-0.7.2/raw-icons/rio/logo-and-text-vertical.svg
+-rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 rio_ui-0.7.2/raw-icons/rio/logo.svg
+-rw-r--r--   0        0        0     5933 2020-02-02 00:00:00.000000 rio_ui-0.7.2/raw-icons/rio/color/logo-and-text-horizontal.svg
+-rw-r--r--   0        0        0     5961 2020-02-02 00:00:00.000000 rio_ui-0.7.2/raw-icons/rio/color/logo-and-text-vertical.svg
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 rio_ui-0.7.2/raw-icons/rio/color/logo.svg
+-rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 rio_ui-0.7.2/raw-icons/rio/fill/logo-and-text-horizontal.svg
+-rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 rio_ui-0.7.2/raw-icons/rio/fill/logo-and-text-vertical.svg
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 rio_ui-0.7.2/raw-icons/rio/fill/logo.svg
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 rio_ui-0.7.2/raw-icons/styling/corner-round-bottom-left.svg
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 rio_ui-0.7.2/raw-icons/styling/corner-round-bottom-right.svg
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 rio_ui-0.7.2/raw-icons/styling/corner-round-top-left.svg
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 rio_ui-0.7.2/raw-icons/styling/corner-round-top-right.svg
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/__init__.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/__main__.py
+-rw-r--r--   0        0        0    19320 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/app.py
+-rw-r--r--   0        0        0    32919 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/app_server.py
+-rw-r--r--   0        0        0     8672 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/assets.py
+-rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/byte_serving.py
+-rw-r--r--   0        0        0    19465 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/color.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/cursor_style.py
+-rw-r--r--   0        0        0     6033 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/dataclass.py
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/errors.py
+-rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/event.py
+-rw-r--r--   0        0        0     6690 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/fills.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/global_state.py
+-rw-r--r--   0        0        0     9857 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/icon_registry.py
+-rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/inspection.py
+-rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/maybes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/py.typed
+-rw-r--r--   0        0        0     8057 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/routing.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/self_serializing.py
+-rw-r--r--   0        0        0     8519 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/serialization.py
+-rw-r--r--   0        0        0    79752 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/session.py
+-rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/session_attachments.py
+-rw-r--r--   0        0        0     8246 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/state_properties.py
+-rw-r--r--   0        0        0     4492 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/text_style.py
+-rw-r--r--   0        0        0    28614 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/theme.py
+-rw-r--r--   0        0        0     5401 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/user_settings_module.py
+-rw-r--r--   0        0        0    10026 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/utils.py
+-rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/world_units.py
+-rw-r--r--   0        0        0    11560 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/assets/fonts/Roboto/LICENSE.txt
+-rw-r--r--   0        0        0   167336 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/assets/fonts/Roboto/Roboto-Bold.ttf
+-rw-r--r--   0        0        0   171508 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/assets/fonts/Roboto/Roboto-BoldItalic.ttf
+-rw-r--r--   0        0        0   170504 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/assets/fonts/Roboto/Roboto-Italic.ttf
+-rw-r--r--   0        0        0   168260 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/assets/fonts/Roboto/Roboto-Regular.ttf
+-rw-r--r--   0        0        0    11560 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/assets/fonts/Roboto Mono/LICENSE.txt
+-rw-r--r--   0        0        0    87392 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/assets/fonts/Roboto Mono/RobotoMono-Bold.ttf
+-rw-r--r--   0        0        0    94636 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/assets/fonts/Roboto Mono/RobotoMono-BoldItalic.ttf
+-rw-r--r--   0        0        0    94372 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/assets/fonts/Roboto Mono/RobotoMono-Italic.ttf
+-rw-r--r--   0        0        0    87236 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/assets/fonts/Roboto Mono/RobotoMono-Regular.ttf
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/assets/hosted/README.md
+-rw-r--r--   0        0        0    54189 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/assets/hosted/rio-logos/logo-and-text-horizontal.png
+-rw-r--r--   0        0        0    31665 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/assets/hosted/rio-logos/rio-logo-square.png
+-rw-r--r--   0        0        0  1081336 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/assets/icon-sets/material.tar.xz
+-rw-r--r--   0        0        0    14992 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/assets/icon-sets/rio.tar.xz
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/assets/icon-sets/styling.tar.xz
+-rw-r--r--   0        0        0     7375 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/cli/__init__.py
+-rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/cli/cli_instance.py
+-rw-r--r--   0        0        0     6672 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/cli/nice_traceback.py
+-rw-r--r--   0        0        0    14016 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/cli/project.py
+-rw-r--r--   0        0        0    14492 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/cli/project_setup.py
+-rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/cli/rio_api.py
+-rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/cli/rioignore.py
+-rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/cli/tomlconfig.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/cli/run_project/__init__.py
+-rw-r--r--   0        0        0     5446 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/cli/run_project/app_loading.py
+-rw-r--r--   0        0        0    22577 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/cli/run_project/arbiter.py
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/cli/run_project/file_watcher_worker.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/cli/run_project/run_models.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/cli/run_project/run_utils.py
+-rw-r--r--   0        0        0     4155 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/cli/run_project/uvicorn_worker.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/cli/run_project/webview_worker.py
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/__init__.py
+-rw-r--r--   0        0        0     4469 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/app_root.py
+-rw-r--r--   0        0        0     4167 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/auto_form.py
+-rw-r--r--   0        0        0     4800 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/banner.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/build_failed.py
+-rw-r--r--   0        0        0    12739 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/button.py
+-rw-r--r--   0        0        0     5325 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/card.py
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/class_container.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/code_block.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/code_explorer.py
+-rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/color_picker.py
+-rw-r--r--   0        0        0    26340 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/component.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/component_tree.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/container.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/debugger_connector.py
+-rw-r--r--   0        0        0     4152 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/devel_component.py
+-rw-r--r--   0        0        0     4274 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/drawer.py
+-rw-r--r--   0        0        0     7070 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/dropdown.py
+-rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/flow_container.py
+-rw-r--r--   0        0        0     6075 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/fundamental_component.py
+-rw-r--r--   0        0        0     7087 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/grid.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/html.py
+-rw-r--r--   0        0        0     7709 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/icon.py
+-rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/image.py
+-rw-r--r--   0        0        0    14169 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/key_event_listener.py
+-rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/labeled_column.py
+-rw-r--r--   0        0        0    10697 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/linear_containers.py
+-rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/link.py
+-rw-r--r--   0        0        0    10524 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/list_items.py
+-rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/list_view.py
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/markdown.py
+-rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/media_player.py
+-rw-r--r--   0        0        0    10800 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/mouse_event_listener.py
+-rw-r--r--   0        0        0     5140 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/multi_line_text_input.py
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/node_input.py
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/node_output.py
+-rw-r--r--   0        0        0     9335 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/number_input.py
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/overlay.py
+-rw-r--r--   0        0        0     5147 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/page_view.py
+-rw-r--r--   0        0        0     4992 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/plot.py
+-rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/popup.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/progress_bar.py
+-rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/progress_circle.py
+-rw-r--r--   0        0        0     5702 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/rectangle.py
+-rw-r--r--   0        0        0     4038 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/revealer.py
+-rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/root_components.py
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/scroll_container.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/scroll_target.py
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/separator.py
+-rw-r--r--   0        0        0     5947 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/slider.py
+-rw-r--r--   0        0        0     3585 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/slideshow.py
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/spacer.py
+-rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/stack.py
+-rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/switch.py
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/switcher.py
+-rw-r--r--   0        0        0     9204 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/switcher_bar.py
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/table.py
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/text.py
+-rw-r--r--   0        0        0     6144 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/text_input.py
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/theme_context_switcher.py
+-rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/tooltip.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/website.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/debug/__init__.py
+-rw-r--r--   0        0        0     7485 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/debug/monkeypatches.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/debug/typing_utils.py
+-rw-r--r--   0        0        0    14479 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/debug/validator.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/debug/dev_tools/__init__.py
+-rw-r--r--   0        0        0    10582 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/debug/dev_tools/component_details.py
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/debug/dev_tools/deploy_page.py
+-rw-r--r--   0        0        0     3598 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/debug/dev_tools/dev_tools_sidebar.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/debug/dev_tools/docs_page.py
+-rw-r--r--   0        0        0    12890 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/debug/dev_tools/icons_page.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/debug/dev_tools/layout_preview.py
+-rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/debug/dev_tools/project_page.py
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/debug/dev_tools/sample_icons_grid.py
+-rw-r--r--   0        0        0    17346 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/debug/dev_tools/theme_picker_page.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/debug/dev_tools/tree_page.py
+-rw-r--r--   0        0        0    10466 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/docs/__init__.py
+-rw-r--r--   0        0        0   416487 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/generated/index.html
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/patches_for_3rd_party_stuff/IocpProactor_accept_locals_accept_coro.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/patches_for_3rd_party_stuff/ProactorBasePipeTransport_call_connection_lost.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/patches_for_3rd_party_stuff/_OverlappedFuture_cancel_overlapped.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/patches_for_3rd_party_stuff/__init__.py
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/README.md
+-rw-r--r--   0        0        0    15602 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/__init__.py
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/howtos/core-classes.md
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/howtos/debugging-setup.md
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/howtos/deployment.md
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/howtos/howto-custom-events.md
+-rw-r--r--   0        0        0     5844 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/howtos/howto-get-value-from-child-component.md
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/howtos/howto-install.md
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/howtos/howto-pass-value-to-event.md
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/howtos/persistent-settings.md
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/howtos/project-setup.md
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/howtos/run-project.md
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/howtos/theming.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/howtos-todo/attribute-bindings.md
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/howtos-todo/component-lifecycle.md
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/howtos-todo/custom-events.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/howtos-todo/force-refresh.md
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/howtos-todo/initialize-component-asynchronously.md
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/howtos-todo/layouting.md
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/howtos-todo/multiple-pages.md
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/other-examples/simple_counter_app.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-AI Chatbot/README.md
+-rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-AI Chatbot/conversation.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-AI Chatbot/meta.json
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-AI Chatbot/root_init.py
+-rw-r--r--   0        0        0   258496 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-AI Chatbot/thumbnail.svg
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-AI Chatbot/components/__init__.py
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_message.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_suggestion_card.py
+-rw-r--r--   0        0        0     3728 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-AI Chatbot/components/empty_chat_placeholder.py
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-AI Chatbot/components/generating_response_placeholder.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-AI Chatbot/pages/__init__.py
+-rw-r--r--   0        0        0     5823 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-AI Chatbot/pages/chat_page.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Crypto Dashboard/README.md
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Crypto Dashboard/data_models.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Crypto Dashboard/meta.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Crypto Dashboard/root_init.py
+-rw-r--r--   0        0        0   270445 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Crypto Dashboard/thumbnail.svg
+-rw-r--r--   0        0        0     7595 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Crypto Dashboard/assets/cryptos.csv
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/__init__.py
+-rw-r--r--   0        0        0    10704 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/balance_card.py
+-rw-r--r--   0        0        0     6695 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_card.py
+-rw-r--r--   0        0        0     5604 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_chart.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Crypto Dashboard/pages/__init__.py
+-rw-r--r--   0        0        0     7668 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Crypto Dashboard/pages/dashboard_page.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Empty/README.md
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Empty/meta.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Empty/root_init.py
+-rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Empty/thumbnail.svg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Empty/pages/__init__.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Empty/pages/sample_page.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Multipage Website/README.md
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Multipage Website/meta.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Multipage Website/root_init.py
+-rw-r--r--   0        0        0   208005 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Multipage Website/thumbnail.svg
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Multipage Website/components/__init__.py
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Multipage Website/components/footer.py
+-rw-r--r--   0        0        0     4826 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Multipage Website/components/navbar.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Multipage Website/components/news_article.py
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Multipage Website/components/testimonial.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Multipage Website/pages/__init__.py
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Multipage Website/pages/about_page.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Multipage Website/pages/home_page.py
+-rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Multipage Website/pages/news_page.py
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Multipage Website/pages/root_page.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Simple CRUD/README.md
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Simple CRUD/data_models.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Simple CRUD/meta.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Simple CRUD/root_init.py
+-rw-r--r--   0        0        0   350009 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Simple CRUD/thumbnail.svg
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Simple CRUD/components/__init__.py
+-rw-r--r--   0        0        0     7284 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_editor.py
+-rw-r--r--   0        0        0     5810 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_list.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Simple CRUD/pages/__init__.py
+-rw-r--r--   0        0        0     8587 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Simple CRUD/pages/crud_page.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/README.md
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/meta.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/root_init.py
+-rw-r--r--   0        0        0    23769 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/thumbnail.svg
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/__init__.py
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/field.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/__init__.py
+-rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/tic_tac_toe_page.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/components/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/__init__.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/tic_tac_toe_page.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/__init__.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/field.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/__init__.py
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/tic_tac_toe_page.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/__init__.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/field.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/__init__.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/tic_tac_toe_page.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/__init__.py
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/field.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/__init__.py
+-rw-r--r--   0        0        0     4348 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/tic_tac_toe_page.py
+-rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 rio_ui-0.7.2/scripts/benchmark.py
+-rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 rio_ui-0.7.2/scripts/build_material_icon_set.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 rio_ui-0.7.2/scripts/cloc.sh
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 rio_ui-0.7.2/scripts/code_coverage.py
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 rio_ui-0.7.2/scripts/publish_new_release.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 rio_ui-0.7.2/tests/test_app_build.py
+-rw-r--r--   0        0        0     8822 2020-02-02 00:00:00.000000 rio_ui-0.7.2/tests/test_attribute_bindings.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 rio_ui-0.7.2/tests/test_custom_components.py
+-rw-r--r--   0        0        0     3426 2020-02-02 00:00:00.000000 rio_ui-0.7.2/tests/test_docstring_code_blocks.py
+-rw-r--r--   0        0        0     3797 2020-02-02 00:00:00.000000 rio_ui-0.7.2/tests/test_documentation.py
+-rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 rio_ui-0.7.2/tests/test_events.py
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 rio_ui-0.7.2/tests/test_project_templates.py
+-rw-r--r--   0        0        0    11737 2020-02-02 00:00:00.000000 rio_ui-0.7.2/tests/test_reconciliation.py
+-rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 rio_ui-0.7.2/tests/test_refresh.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 rio_ui-0.7.2/tests/test_session.py
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 rio_ui-0.7.2/tests/test_user_settings.py
+-rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 rio_ui-0.7.2/tests/test_zzz_guardrails.py
+-rw-r--r--   0        0        0     8596 2020-02-02 00:00:00.000000 rio_ui-0.7.2/tests/utils.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 rio_ui-0.7.2/.gitignore
+-rw-r--r--   0        0        0    11315 2020-02-02 00:00:00.000000 rio_ui-0.7.2/LICENSE.txt
+-rw-r--r--   0        0        0     7523 2020-02-02 00:00:00.000000 rio_ui-0.7.2/README.md
+-rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 rio_ui-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0    22744 2020-02-02 00:00:00.000000 rio_ui-0.7.2/PKG-INFO
```

### Comparing `rio_ui-0.7.1/CODE_OF_CONDUCT.md` & `rio_ui-0.7.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/CONTRIBUTING.md` & `rio_ui-0.7.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/package.json` & `rio_ui-0.7.2/package.json`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/.github/ISSUE_TEMPLATE/bug_report.yml` & `rio_ui-0.7.2/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/index.html` & `rio_ui-0.7.2/frontend/index.html`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/app.ts` & `rio_ui-0.7.2/frontend/code/app.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/colorConversion.ts` & `rio_ui-0.7.2/frontend/code/colorConversion.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/componentManagement.ts` & `rio_ui-0.7.2/frontend/code/componentManagement.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/cssUtils.ts` & `rio_ui-0.7.2/frontend/code/cssUtils.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/dataModels.ts` & `rio_ui-0.7.2/frontend/code/dataModels.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/designApplication.ts` & `rio_ui-0.7.2/frontend/code/designApplication.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/easeFunctions.ts` & `rio_ui-0.7.2/frontend/code/easeFunctions.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/eventHandling.ts` & `rio_ui-0.7.2/frontend/code/eventHandling.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/inputBoxTools.ts` & `rio_ui-0.7.2/frontend/code/inputBoxTools.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/layoutHelpers.ts` & `rio_ui-0.7.2/frontend/code/layoutHelpers.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/layouting.ts` & `rio_ui-0.7.2/frontend/code/layouting.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/rippleEffect.ts` & `rio_ui-0.7.2/frontend/code/rippleEffect.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/rpc.ts` & `rio_ui-0.7.2/frontend/code/rpc.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/rpcFunctions.ts` & `rio_ui-0.7.2/frontend/code/rpcFunctions.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/utils.ts` & `rio_ui-0.7.2/frontend/code/utils.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/components/align.ts` & `rio_ui-0.7.2/frontend/code/components/align.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/components/buildFailed.ts` & `rio_ui-0.7.2/frontend/code/components/buildFailed.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/components/button.ts` & `rio_ui-0.7.2/frontend/code/components/button.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/components/card.ts` & `rio_ui-0.7.2/frontend/code/components/card.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/components/classContainer.ts` & `rio_ui-0.7.2/frontend/code/components/classContainer.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/components/codeBlock.ts` & `rio_ui-0.7.2/frontend/code/components/codeBlock.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/components/codeExplorer.ts` & `rio_ui-0.7.2/frontend/code/components/codeExplorer.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/components/colorPicker.ts` & `rio_ui-0.7.2/frontend/code/components/colorPicker.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/components/componentBase.ts` & `rio_ui-0.7.2/frontend/code/components/componentBase.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/components/componentTree.ts` & `rio_ui-0.7.2/frontend/code/components/componentTree.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/components/customListItem.ts` & `rio_ui-0.7.2/frontend/code/components/customListItem.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/components/debuggerConnector.ts` & `rio_ui-0.7.2/frontend/code/components/debuggerConnector.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/components/drawer.ts` & `rio_ui-0.7.2/frontend/code/components/drawer.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/components/dropdown.ts` & `rio_ui-0.7.2/frontend/code/components/dropdown.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/components/flowContainer.ts` & `rio_ui-0.7.2/frontend/code/components/flowContainer.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/components/fundamentalRootComponent.ts` & `rio_ui-0.7.2/frontend/code/components/fundamentalRootComponent.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/components/grid.ts` & `rio_ui-0.7.2/frontend/code/components/grid.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/components/headingListItem.ts` & `rio_ui-0.7.2/frontend/code/components/headingListItem.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/components/html.ts` & `rio_ui-0.7.2/frontend/code/components/html.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/components/icon.ts` & `rio_ui-0.7.2/frontend/code/components/icon.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/components/image.ts` & `rio_ui-0.7.2/frontend/code/components/image.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/components/keyEventListener.ts` & `rio_ui-0.7.2/frontend/code/components/keyEventListener.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/components/linearContainers.ts` & `rio_ui-0.7.2/frontend/code/components/linearContainers.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/components/link.ts` & `rio_ui-0.7.2/frontend/code/components/link.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/components/listView.ts` & `rio_ui-0.7.2/frontend/code/components/listView.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/components/margin.ts` & `rio_ui-0.7.2/frontend/code/components/margin.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/components/markdown.ts` & `rio_ui-0.7.2/frontend/code/components/markdown.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/components/mediaPlayer.ts` & `rio_ui-0.7.2/frontend/code/components/mediaPlayer.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/components/mouseEventListener.ts` & `rio_ui-0.7.2/frontend/code/components/mouseEventListener.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/components/multiLineTextInput.ts` & `rio_ui-0.7.2/frontend/code/components/multiLineTextInput.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/components/nodeInput.ts` & `rio_ui-0.7.2/frontend/code/components/nodeInput.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/components/nodeOutput.ts` & `rio_ui-0.7.2/frontend/code/components/nodeOutput.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/components/overlay.ts` & `rio_ui-0.7.2/frontend/code/components/overlay.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/components/placeholder.ts` & `rio_ui-0.7.2/frontend/code/components/placeholder.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/components/plot.ts` & `rio_ui-0.7.2/frontend/code/components/plot.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/components/popup.ts` & `rio_ui-0.7.2/frontend/code/components/popup.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/components/progressBar.ts` & `rio_ui-0.7.2/frontend/code/components/progressBar.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/components/progressCircle.ts` & `rio_ui-0.7.2/frontend/code/components/progressCircle.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/components/rectangle.ts` & `rio_ui-0.7.2/frontend/code/components/rectangle.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/components/revealer.ts` & `rio_ui-0.7.2/frontend/code/components/revealer.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/components/scrollContainer.ts` & `rio_ui-0.7.2/frontend/code/components/scrollContainer.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/components/scrollTarget.ts` & `rio_ui-0.7.2/frontend/code/components/scrollTarget.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/components/separator.ts` & `rio_ui-0.7.2/frontend/code/components/separator.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/components/separatorListItem.ts` & `rio_ui-0.7.2/frontend/code/components/separatorListItem.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/components/singleContainer.ts` & `rio_ui-0.7.2/frontend/code/components/singleContainer.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/components/slider.ts` & `rio_ui-0.7.2/frontend/code/components/slider.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/components/slideshow.ts` & `rio_ui-0.7.2/frontend/code/components/slideshow.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/components/stack.ts` & `rio_ui-0.7.2/frontend/code/components/stack.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/components/switch.ts` & `rio_ui-0.7.2/frontend/code/components/switch.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/components/switcher.ts` & `rio_ui-0.7.2/frontend/code/components/switcher.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/components/switcherBar.ts` & `rio_ui-0.7.2/frontend/code/components/switcherBar.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/components/table.ts` & `rio_ui-0.7.2/frontend/code/components/table.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/components/text.ts` & `rio_ui-0.7.2/frontend/code/components/text.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/components/textInput.ts` & `rio_ui-0.7.2/frontend/code/components/textInput.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/components/themeContextSwitcher.ts` & `rio_ui-0.7.2/frontend/code/components/themeContextSwitcher.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/components/tooltip.ts` & `rio_ui-0.7.2/frontend/code/components/tooltip.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/code/components/website.ts` & `rio_ui-0.7.2/frontend/code/components/website.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/css/highlightjs-default-dark.css` & `rio_ui-0.7.2/frontend/css/highlightjs-default-dark.css`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/css/highlightjs-default-light.css` & `rio_ui-0.7.2/frontend/css/highlightjs-default-light.css`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/css/style.scss` & `rio_ui-0.7.2/frontend/css/style.scss`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/frontend/css/switcheroos.scss` & `rio_ui-0.7.2/frontend/css/switcheroos.scss`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/raw-icons/custom-material-icons/twinkle.svg` & `rio_ui-0.7.2/raw-icons/custom-material-icons/twinkle.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/raw-icons/custom-material-icons/fill/twinkle.svg` & `rio_ui-0.7.2/raw-icons/custom-material-icons/fill/twinkle.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/raw-icons/rio/logo-and-text-horizontal.svg` & `rio_ui-0.7.2/raw-icons/rio/logo-and-text-horizontal.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/raw-icons/rio/logo-and-text-vertical.svg` & `rio_ui-0.7.2/raw-icons/rio/logo-and-text-vertical.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/raw-icons/rio/logo.svg` & `rio_ui-0.7.2/raw-icons/rio/logo.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/raw-icons/rio/color/logo-and-text-horizontal.svg` & `rio_ui-0.7.2/raw-icons/rio/color/logo-and-text-horizontal.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/raw-icons/rio/color/logo-and-text-vertical.svg` & `rio_ui-0.7.2/raw-icons/rio/color/logo-and-text-vertical.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/raw-icons/rio/color/logo.svg` & `rio_ui-0.7.2/raw-icons/rio/color/logo.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/raw-icons/rio/fill/logo-and-text-horizontal.svg` & `rio_ui-0.7.2/raw-icons/rio/fill/logo-and-text-horizontal.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/raw-icons/rio/fill/logo-and-text-vertical.svg` & `rio_ui-0.7.2/raw-icons/rio/fill/logo-and-text-vertical.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/raw-icons/rio/fill/logo.svg` & `rio_ui-0.7.2/raw-icons/rio/fill/logo.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/raw-icons/styling/corner-round-bottom-left.svg` & `rio_ui-0.7.2/raw-icons/styling/corner-round-bottom-left.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/raw-icons/styling/corner-round-bottom-right.svg` & `rio_ui-0.7.2/raw-icons/styling/corner-round-bottom-right.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/raw-icons/styling/corner-round-top-left.svg` & `rio_ui-0.7.2/raw-icons/styling/corner-round-top-left.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/raw-icons/styling/corner-round-top-right.svg` & `rio_ui-0.7.2/raw-icons/styling/corner-round-top-right.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/__init__.py` & `rio_ui-0.7.2/rio/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.7.1"
+__version__ = "0.7.2"
 
 import logging
 
 _logger = logging.getLogger(__name__)
 
 # Re-export dataclass stuff for easy use.
 from dataclasses import KW_ONLY as KW_ONLY
```

### Comparing `rio_ui-0.7.1/rio/app.py` & `rio_ui-0.7.2/rio/app.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/app_server.py` & `rio_ui-0.7.2/rio/app_server.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/assets.py` & `rio_ui-0.7.2/rio/assets.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/byte_serving.py` & `rio_ui-0.7.2/rio/byte_serving.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/color.py` & `rio_ui-0.7.2/rio/color.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/dataclass.py` & `rio_ui-0.7.2/rio/dataclass.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/errors.py` & `rio_ui-0.7.2/rio/errors.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/event.py` & `rio_ui-0.7.2/rio/event.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/fills.py` & `rio_ui-0.7.2/rio/fills.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/global_state.py` & `rio_ui-0.7.2/rio/global_state.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/icon_registry.py` & `rio_ui-0.7.2/rio/icon_registry.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/inspection.py` & `rio_ui-0.7.2/rio/inspection.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/maybes.py` & `rio_ui-0.7.2/rio/maybes.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/routing.py` & `rio_ui-0.7.2/rio/routing.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/serialization.py` & `rio_ui-0.7.2/rio/serialization.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/session.py` & `rio_ui-0.7.2/rio/session.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/session_attachments.py` & `rio_ui-0.7.2/rio/session_attachments.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/state_properties.py` & `rio_ui-0.7.2/rio/state_properties.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/text_style.py` & `rio_ui-0.7.2/rio/text_style.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/theme.py` & `rio_ui-0.7.2/rio/theme.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/user_settings_module.py` & `rio_ui-0.7.2/rio/user_settings_module.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/utils.py` & `rio_ui-0.7.2/rio/utils.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/world_units.py` & `rio_ui-0.7.2/rio/world_units.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/assets/fonts/Roboto/LICENSE.txt` & `rio_ui-0.7.2/rio/assets/fonts/Roboto/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/assets/fonts/Roboto/Roboto-Bold.ttf` & `rio_ui-0.7.2/rio/assets/fonts/Roboto/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/assets/fonts/Roboto/Roboto-BoldItalic.ttf` & `rio_ui-0.7.2/rio/assets/fonts/Roboto/Roboto-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/assets/fonts/Roboto/Roboto-Italic.ttf` & `rio_ui-0.7.2/rio/assets/fonts/Roboto/Roboto-Italic.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/assets/fonts/Roboto/Roboto-Regular.ttf` & `rio_ui-0.7.2/rio/assets/fonts/Roboto/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/assets/fonts/Roboto Mono/LICENSE.txt` & `rio_ui-0.7.2/rio/assets/fonts/Roboto Mono/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/assets/fonts/Roboto Mono/RobotoMono-Bold.ttf` & `rio_ui-0.7.2/rio/assets/fonts/Roboto Mono/RobotoMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/assets/fonts/Roboto Mono/RobotoMono-BoldItalic.ttf` & `rio_ui-0.7.2/rio/assets/fonts/Roboto Mono/RobotoMono-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/assets/fonts/Roboto Mono/RobotoMono-Italic.ttf` & `rio_ui-0.7.2/rio/assets/fonts/Roboto Mono/RobotoMono-Italic.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/assets/fonts/Roboto Mono/RobotoMono-Regular.ttf` & `rio_ui-0.7.2/rio/assets/fonts/Roboto Mono/RobotoMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/assets/hosted/rio-logos/logo-and-text-horizontal.png` & `rio_ui-0.7.2/rio/assets/hosted/rio-logos/logo-and-text-horizontal.png`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/assets/hosted/rio-logos/rio-logo-square.png` & `rio_ui-0.7.2/rio/assets/hosted/rio-logos/rio-logo-square.png`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/assets/icon-sets/material.tar.xz` & `rio_ui-0.7.2/rio/assets/icon-sets/material.tar.xz`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/assets/icon-sets/rio.tar.xz` & `rio_ui-0.7.2/rio/assets/icon-sets/rio.tar.xz`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/assets/icon-sets/styling.tar.xz` & `rio_ui-0.7.2/rio/assets/icon-sets/styling.tar.xz`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/cli/__init__.py` & `rio_ui-0.7.2/rio/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/cli/cli_instance.py` & `rio_ui-0.7.2/rio/cli/cli_instance.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/cli/nice_traceback.py` & `rio_ui-0.7.2/rio/cli/nice_traceback.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/cli/project.py` & `rio_ui-0.7.2/rio/cli/project.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/cli/project_setup.py` & `rio_ui-0.7.2/rio/cli/project_setup.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/cli/rio_api.py` & `rio_ui-0.7.2/rio/cli/rio_api.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/cli/rioignore.py` & `rio_ui-0.7.2/rio/cli/rioignore.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/cli/tomlconfig.py` & `rio_ui-0.7.2/rio/cli/tomlconfig.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/cli/run_project/app_loading.py` & `rio_ui-0.7.2/rio/cli/run_project/app_loading.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/cli/run_project/arbiter.py` & `rio_ui-0.7.2/rio/cli/run_project/arbiter.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/cli/run_project/file_watcher_worker.py` & `rio_ui-0.7.2/rio/cli/run_project/file_watcher_worker.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/cli/run_project/uvicorn_worker.py` & `rio_ui-0.7.2/rio/cli/run_project/uvicorn_worker.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/cli/run_project/webview_worker.py` & `rio_ui-0.7.2/rio/cli/run_project/webview_worker.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/__init__.py` & `rio_ui-0.7.2/rio/components/__init__.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/app_root.py` & `rio_ui-0.7.2/rio/components/app_root.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/auto_form.py` & `rio_ui-0.7.2/rio/components/auto_form.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/banner.py` & `rio_ui-0.7.2/rio/components/banner.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/build_failed.py` & `rio_ui-0.7.2/rio/components/build_failed.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/button.py` & `rio_ui-0.7.2/rio/components/button.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/card.py` & `rio_ui-0.7.2/rio/components/card.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/class_container.py` & `rio_ui-0.7.2/rio/components/class_container.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/code_block.py` & `rio_ui-0.7.2/rio/components/code_block.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/color_picker.py` & `rio_ui-0.7.2/rio/components/color_picker.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/component.py` & `rio_ui-0.7.2/rio/components/component.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/component_tree.py` & `rio_ui-0.7.2/rio/components/component_tree.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/container.py` & `rio_ui-0.7.2/rio/components/container.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/devel_component.py` & `rio_ui-0.7.2/rio/components/devel_component.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/drawer.py` & `rio_ui-0.7.2/rio/components/drawer.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/dropdown.py` & `rio_ui-0.7.2/rio/components/dropdown.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/flow_container.py` & `rio_ui-0.7.2/rio/components/flow_container.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/fundamental_component.py` & `rio_ui-0.7.2/rio/components/fundamental_component.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/grid.py` & `rio_ui-0.7.2/rio/components/grid.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/html.py` & `rio_ui-0.7.2/rio/components/html.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/icon.py` & `rio_ui-0.7.2/rio/components/icon.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/image.py` & `rio_ui-0.7.2/rio/components/image.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/key_event_listener.py` & `rio_ui-0.7.2/rio/components/key_event_listener.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/labeled_column.py` & `rio_ui-0.7.2/rio/components/labeled_column.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/linear_containers.py` & `rio_ui-0.7.2/rio/components/linear_containers.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/link.py` & `rio_ui-0.7.2/rio/components/link.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/list_items.py` & `rio_ui-0.7.2/rio/components/list_items.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/list_view.py` & `rio_ui-0.7.2/rio/components/list_view.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/markdown.py` & `rio_ui-0.7.2/rio/components/markdown.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/media_player.py` & `rio_ui-0.7.2/rio/components/media_player.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/mouse_event_listener.py` & `rio_ui-0.7.2/rio/components/mouse_event_listener.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/multi_line_text_input.py` & `rio_ui-0.7.2/rio/components/multi_line_text_input.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/node_input.py` & `rio_ui-0.7.2/rio/components/node_input.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/node_output.py` & `rio_ui-0.7.2/rio/components/node_output.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/number_input.py` & `rio_ui-0.7.2/rio/components/number_input.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/overlay.py` & `rio_ui-0.7.2/rio/components/overlay.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/page_view.py` & `rio_ui-0.7.2/rio/components/page_view.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/plot.py` & `rio_ui-0.7.2/rio/components/plot.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/popup.py` & `rio_ui-0.7.2/rio/components/popup.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/progress_bar.py` & `rio_ui-0.7.2/rio/components/progress_bar.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/progress_circle.py` & `rio_ui-0.7.2/rio/components/progress_circle.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/rectangle.py` & `rio_ui-0.7.2/rio/components/rectangle.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/revealer.py` & `rio_ui-0.7.2/rio/components/revealer.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/root_components.py` & `rio_ui-0.7.2/rio/components/root_components.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/scroll_container.py` & `rio_ui-0.7.2/rio/components/scroll_container.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/scroll_target.py` & `rio_ui-0.7.2/rio/components/scroll_target.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/separator.py` & `rio_ui-0.7.2/rio/components/separator.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/slider.py` & `rio_ui-0.7.2/rio/components/slider.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/slideshow.py` & `rio_ui-0.7.2/rio/components/slideshow.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/spacer.py` & `rio_ui-0.7.2/rio/components/spacer.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/stack.py` & `rio_ui-0.7.2/rio/components/stack.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/switch.py` & `rio_ui-0.7.2/rio/components/switch.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/switcher.py` & `rio_ui-0.7.2/rio/components/switcher.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/switcher_bar.py` & `rio_ui-0.7.2/rio/components/switcher_bar.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/table.py` & `rio_ui-0.7.2/rio/components/table.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/text.py` & `rio_ui-0.7.2/rio/components/text.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/text_input.py` & `rio_ui-0.7.2/rio/components/text_input.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/theme_context_switcher.py` & `rio_ui-0.7.2/rio/components/theme_context_switcher.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/tooltip.py` & `rio_ui-0.7.2/rio/components/tooltip.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/components/website.py` & `rio_ui-0.7.2/rio/components/website.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/debug/monkeypatches.py` & `rio_ui-0.7.2/rio/debug/monkeypatches.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/debug/typing_utils.py` & `rio_ui-0.7.2/rio/debug/typing_utils.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/debug/validator.py` & `rio_ui-0.7.2/rio/debug/validator.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/debug/dev_tools/component_details.py` & `rio_ui-0.7.2/rio/debug/dev_tools/component_details.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/debug/dev_tools/deploy_page.py` & `rio_ui-0.7.2/rio/debug/dev_tools/deploy_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/debug/dev_tools/dev_tools_sidebar.py` & `rio_ui-0.7.2/rio/debug/dev_tools/dev_tools_sidebar.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/debug/dev_tools/docs_page.py` & `rio_ui-0.7.2/rio/debug/dev_tools/docs_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/debug/dev_tools/icons_page.py` & `rio_ui-0.7.2/rio/debug/dev_tools/icons_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/debug/dev_tools/layout_preview.py` & `rio_ui-0.7.2/rio/debug/dev_tools/layout_preview.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/debug/dev_tools/project_page.py` & `rio_ui-0.7.2/rio/debug/dev_tools/project_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/debug/dev_tools/sample_icons_grid.py` & `rio_ui-0.7.2/rio/debug/dev_tools/sample_icons_grid.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/debug/dev_tools/theme_picker_page.py` & `rio_ui-0.7.2/rio/debug/dev_tools/theme_picker_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/debug/dev_tools/tree_page.py` & `rio_ui-0.7.2/rio/debug/dev_tools/tree_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/docs/__init__.py` & `rio_ui-0.7.2/rio/docs/__init__.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/generated/index.html` & `rio_ui-0.7.2/rio/generated/index.html`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/patches_for_3rd_party_stuff/IocpProactor_accept_locals_accept_coro.py` & `rio_ui-0.7.2/rio/patches_for_3rd_party_stuff/IocpProactor_accept_locals_accept_coro.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/patches_for_3rd_party_stuff/ProactorBasePipeTransport_call_connection_lost.py` & `rio_ui-0.7.2/rio/patches_for_3rd_party_stuff/ProactorBasePipeTransport_call_connection_lost.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/patches_for_3rd_party_stuff/_OverlappedFuture_cancel_overlapped.py` & `rio_ui-0.7.2/rio/patches_for_3rd_party_stuff/_OverlappedFuture_cancel_overlapped.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/README.md` & `rio_ui-0.7.2/rio/snippets/README.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/__init__.py` & `rio_ui-0.7.2/rio/snippets/__init__.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/snippet-files/howtos/core-classes.md` & `rio_ui-0.7.2/rio/snippets/snippet-files/howtos/core-classes.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/snippet-files/howtos/debugging-setup.md` & `rio_ui-0.7.2/rio/snippets/snippet-files/howtos/debugging-setup.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/snippet-files/howtos/deployment.md` & `rio_ui-0.7.2/rio/snippets/snippet-files/howtos/deployment.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/snippet-files/howtos/howto-custom-events.md` & `rio_ui-0.7.2/rio/snippets/snippet-files/howtos/howto-custom-events.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/snippet-files/howtos/howto-get-value-from-child-component.md` & `rio_ui-0.7.2/rio/snippets/snippet-files/howtos/howto-get-value-from-child-component.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/snippet-files/howtos/howto-install.md` & `rio_ui-0.7.2/rio/snippets/snippet-files/howtos/howto-install.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/snippet-files/howtos/howto-pass-value-to-event.md` & `rio_ui-0.7.2/rio/snippets/snippet-files/howtos/howto-pass-value-to-event.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/snippet-files/howtos/persistent-settings.md` & `rio_ui-0.7.2/rio/snippets/snippet-files/howtos/persistent-settings.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/snippet-files/howtos/project-setup.md` & `rio_ui-0.7.2/rio/snippets/snippet-files/howtos/project-setup.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/snippet-files/howtos/run-project.md` & `rio_ui-0.7.2/rio/snippets/snippet-files/howtos/run-project.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/snippet-files/howtos/theming.md` & `rio_ui-0.7.2/rio/snippets/snippet-files/howtos/theming.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/snippet-files/other-examples/simple_counter_app.py` & `rio_ui-0.7.2/rio/snippets/snippet-files/other-examples/simple_counter_app.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/snippet-files/project-template-AI Chatbot/README.md` & `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-AI Chatbot/README.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/snippet-files/project-template-AI Chatbot/conversation.py` & `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-AI Chatbot/conversation.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/snippet-files/project-template-AI Chatbot/root_init.py` & `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-AI Chatbot/root_init.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/snippet-files/project-template-AI Chatbot/thumbnail.svg` & `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-AI Chatbot/thumbnail.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_message.py` & `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_message.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_suggestion_card.py` & `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_suggestion_card.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/snippet-files/project-template-AI Chatbot/components/empty_chat_placeholder.py` & `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-AI Chatbot/components/empty_chat_placeholder.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/snippet-files/project-template-AI Chatbot/components/generating_response_placeholder.py` & `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-AI Chatbot/components/generating_response_placeholder.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/snippet-files/project-template-AI Chatbot/pages/chat_page.py` & `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-AI Chatbot/pages/chat_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Crypto Dashboard/README.md` & `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Crypto Dashboard/README.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Crypto Dashboard/data_models.py` & `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Crypto Dashboard/data_models.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Crypto Dashboard/thumbnail.svg` & `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Crypto Dashboard/thumbnail.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Crypto Dashboard/assets/cryptos.csv` & `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Crypto Dashboard/assets/cryptos.csv`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/balance_card.py` & `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/balance_card.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_card.py` & `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_card.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_chart.py` & `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_chart.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Crypto Dashboard/pages/dashboard_page.py` & `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Crypto Dashboard/pages/dashboard_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Empty/thumbnail.svg` & `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Empty/thumbnail.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Empty/pages/sample_page.py` & `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Empty/pages/sample_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Multipage Website/README.md` & `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Multipage Website/README.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Multipage Website/thumbnail.svg` & `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Multipage Website/thumbnail.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Multipage Website/components/footer.py` & `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Multipage Website/components/footer.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Multipage Website/components/navbar.py` & `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Multipage Website/components/navbar.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Multipage Website/components/testimonial.py` & `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Multipage Website/components/testimonial.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Multipage Website/pages/about_page.py` & `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Multipage Website/pages/about_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Multipage Website/pages/home_page.py` & `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Multipage Website/pages/home_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Multipage Website/pages/news_page.py` & `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Multipage Website/pages/news_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Multipage Website/pages/root_page.py` & `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Multipage Website/pages/root_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Simple CRUD/README.md` & `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Simple CRUD/README.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Simple CRUD/data_models.py` & `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Simple CRUD/data_models.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Simple CRUD/thumbnail.svg` & `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Simple CRUD/thumbnail.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_editor.py` & `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_editor.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_list.py` & `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_list.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Simple CRUD/pages/crud_page.py` & `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Simple CRUD/pages/crud_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/thumbnail.svg` & `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/thumbnail.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/field.py` & `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/field.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/tic_tac_toe_page.py` & `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/tic_tac_toe_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/tic_tac_toe_page.py` & `rio_ui-0.7.2/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/tic_tac_toe_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/field.py` & `rio_ui-0.7.2/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/field.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/tic_tac_toe_page.py` & `rio_ui-0.7.2/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/tic_tac_toe_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/field.py` & `rio_ui-0.7.2/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/field.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/tic_tac_toe_page.py` & `rio_ui-0.7.2/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/tic_tac_toe_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/field.py` & `rio_ui-0.7.2/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/field.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/tic_tac_toe_page.py` & `rio_ui-0.7.2/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/tic_tac_toe_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/scripts/benchmark.py` & `rio_ui-0.7.2/scripts/benchmark.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/scripts/build_material_icon_set.py` & `rio_ui-0.7.2/scripts/build_material_icon_set.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/scripts/code_coverage.py` & `rio_ui-0.7.2/scripts/code_coverage.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/scripts/publish_new_release.py` & `rio_ui-0.7.2/scripts/publish_new_release.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/tests/test_attribute_bindings.py` & `rio_ui-0.7.2/tests/test_attribute_bindings.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/tests/test_custom_components.py` & `rio_ui-0.7.2/tests/test_custom_components.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/tests/test_docstring_code_blocks.py` & `rio_ui-0.7.2/tests/test_docstring_code_blocks.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/tests/test_documentation.py` & `rio_ui-0.7.2/tests/test_documentation.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/tests/test_events.py` & `rio_ui-0.7.2/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/tests/test_project_templates.py` & `rio_ui-0.7.2/tests/test_project_templates.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/tests/test_reconciliation.py` & `rio_ui-0.7.2/tests/test_reconciliation.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/tests/test_refresh.py` & `rio_ui-0.7.2/tests/test_refresh.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/tests/test_session.py` & `rio_ui-0.7.2/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/tests/test_user_settings.py` & `rio_ui-0.7.2/tests/test_user_settings.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/tests/test_zzz_guardrails.py` & `rio_ui-0.7.2/tests/test_zzz_guardrails.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/tests/utils.py` & `rio_ui-0.7.2/tests/utils.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/LICENSE.txt` & `rio_ui-0.7.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/README.md` & `rio_ui-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.1/pyproject.toml` & `rio_ui-0.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -12,30 +12,30 @@
     "fuzzywuzzy~=0.18.0",
     "gitignore-parser~=0.1.9",
     "httpx~=0.25.1",
     "imy~=0.3.2",
     "introspection~=1.8",
     "isort~=5.13.2",
     "keyring~=24.3.0",
+    "matplotlib>=3.8.4",
     "pillow~=10.2.0",
+    "plotly>=5.22.0",
     "pytest~=7.3.1",
     "python-levenshtein~=0.23.0",
     "python-multipart~=0.0.6",
     "pytz~=2024.1",
-    "revel~=0.9.0",
+    "revel~=0.9.1",
     "timer-dict~=1.0.0",
     "tomlkit~=0.12.3",
     "typing-extensions>=4.5.0",
     "unicall~=0.1.5",
     "uniserde~=0.3.13",
     "uvicorn[standard]~=0.23.2",
     "watchfiles~=0.21.0",
     "yarl>=1.9.4",
-    "plotly>=5.22.0",
-    "matplotlib>=3.8.4",
 ]
 requires-python = ">= 3.10"
 readme = "README.md"
 license.file = "LICENSE.txt"
 keywords = [
     "web-development",
     "web-framework",
```

### Comparing `rio_ui-0.7.1/PKG-INFO` & `rio_ui-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: rio-ui
-Version: 0.7.1
+Version: 0.7.2
 Summary: Build modern Websites and Apps just with Python
 Project-URL: homepage, https://rio.dev
 Project-URL: documentation, https://rio.dev/docs
 Author-email: Jakob Pinterits <jakob.pinterits@gmail.com>, Paul Pinterits <rawing7@gmail.com>
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -233,15 +233,15 @@
 Requires-Dist: matplotlib>=3.8.4
 Requires-Dist: pillow~=10.2.0
 Requires-Dist: plotly>=5.22.0
 Requires-Dist: pytest~=7.3.1
 Requires-Dist: python-levenshtein~=0.23.0
 Requires-Dist: python-multipart~=0.0.6
 Requires-Dist: pytz~=2024.1
-Requires-Dist: revel~=0.9.0
+Requires-Dist: revel~=0.9.1
 Requires-Dist: timer-dict~=1.0.0
 Requires-Dist: tomlkit~=0.12.3
 Requires-Dist: typing-extensions>=4.5.0
 Requires-Dist: unicall~=0.1.5
 Requires-Dist: uniserde~=0.3.13
 Requires-Dist: uvicorn[standard]~=0.23.2
 Requires-Dist: watchfiles~=0.21.0
```

