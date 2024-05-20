# Comparing `tmp/rio_ui-0.7.2.tar.gz` & `tmp/rio_ui-0.7.3.tar.gz`

## Comparing `rio_ui-0.7.2.tar` & `rio_ui-0.7.3.tar`

### file list

```diff
@@ -1,365 +1,381 @@
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 rio_ui-0.7.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 rio_ui-0.7.2/.prettierrc
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 rio_ui-0.7.2/.sassrc
--rw-r--r--   0        0        0     5534 2020-02-02 00:00:00.000000 rio_ui-0.7.2/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 rio_ui-0.7.2/CONTRIBUTING.md
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 rio_ui-0.7.2/changelog.md
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 rio_ui-0.7.2/package.json
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 rio_ui-0.7.2/vite.config.js
--rw-r--r--   0        0        0     5140 2020-02-02 00:00:00.000000 rio_ui-0.7.2/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/index.html
--rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/app.ts
--rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/colorConversion.ts
--rw-r--r--   0        0        0    20706 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/componentManagement.ts
--rw-r--r--   0        0        0     5795 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/cssUtils.ts
--rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/dataModels.ts
--rw-r--r--   0        0        0     6925 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/designApplication.ts
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/easeFunctions.ts
--rw-r--r--   0        0        0     4869 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/eventHandling.ts
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/inputBoxTools.ts
--rw-r--r--   0        0        0     6081 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/layoutHelpers.ts
--rw-r--r--   0        0        0     4878 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/layouting.ts
--rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/rippleEffect.ts
--rw-r--r--   0        0        0    11646 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/rpc.ts
--rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/rpcFunctions.ts
--rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/utils.ts
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/align.ts
--rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/buildFailed.ts
--rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/button.ts
--rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/card.ts
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/classContainer.ts
--rw-r--r--   0        0        0     6349 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/codeBlock.ts
--rw-r--r--   0        0        0    15146 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/codeExplorer.ts
--rw-r--r--   0        0        0    13820 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/colorPicker.ts
--rw-r--r--   0        0        0    13570 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/componentBase.ts
--rw-r--r--   0        0        0    14334 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/componentTree.ts
--rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/customListItem.ts
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/debuggerConnector.ts
--rw-r--r--   0        0        0    11400 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/drawer.ts
--rw-r--r--   0        0        0    16927 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/dropdown.ts
--rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/flowContainer.ts
--rw-r--r--   0        0        0     5700 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/fundamentalRootComponent.ts
--rw-r--r--   0        0        0    11004 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/grid.ts
--rw-r--r--   0        0        0     2201 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/headingListItem.ts
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/html.ts
--rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/icon.ts
--rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/image.ts
--rw-r--r--   0        0        0    19839 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/keyEventListener.ts
--rw-r--r--   0        0        0     9923 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/linearContainers.ts
--rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/link.ts
--rw-r--r--   0        0        0     4575 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/listView.ts
--rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/margin.ts
--rw-r--r--   0        0        0     6268 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/markdown.ts
--rw-r--r--   0        0        0    27995 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/mediaPlayer.ts
--rw-r--r--   0        0        0     5948 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/mouseEventListener.ts
--rw-r--r--   0        0        0     4122 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/multiLineTextInput.ts
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/nodeInput.ts
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/nodeOutput.ts
--rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/overlay.ts
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/placeholder.ts
--rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/plot.ts
--rw-r--r--   0        0        0     7055 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/popup.ts
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/progressBar.ts
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/progressCircle.ts
--rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/rectangle.ts
--rw-r--r--   0        0        0    10840 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/revealer.ts
--rw-r--r--   0        0        0     9454 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/scrollContainer.ts
--rw-r--r--   0        0        0     6620 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/scrollTarget.ts
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/separator.ts
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/separatorListItem.ts
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/singleContainer.ts
--rw-r--r--   0        0        0     5031 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/slider.ts
--rw-r--r--   0        0        0     7104 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/slideshow.ts
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/stack.ts
--rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/switch.ts
--rw-r--r--   0        0        0     8056 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/switcher.ts
--rw-r--r--   0        0        0    19999 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/switcherBar.ts
--rw-r--r--   0        0        0     8067 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/table.ts
--rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/text.ts
--rw-r--r--   0        0        0     7311 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/textInput.ts
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/themeContextSwitcher.ts
--rw-r--r--   0        0        0     4463 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/tooltip.ts
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/code/components/website.ts
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/css/highlightjs-default-dark.css
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/css/highlightjs-default-light.css
--rw-r--r--   0        0        0    50930 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/css/style.scss
--rw-r--r--   0        0        0     8244 2020-02-02 00:00:00.000000 rio_ui-0.7.2/frontend/css/switcheroos.scss
--rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 rio_ui-0.7.2/raw-icons/custom-material-icons/twinkle.svg
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 rio_ui-0.7.2/raw-icons/custom-material-icons/fill/twinkle.svg
--rw-r--r--   0        0        0    10067 2020-02-02 00:00:00.000000 rio_ui-0.7.2/raw-icons/rio/logo-and-text-horizontal.svg
--rw-r--r--   0        0        0    10127 2020-02-02 00:00:00.000000 rio_ui-0.7.2/raw-icons/rio/logo-and-text-vertical.svg
--rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 rio_ui-0.7.2/raw-icons/rio/logo.svg
--rw-r--r--   0        0        0     5933 2020-02-02 00:00:00.000000 rio_ui-0.7.2/raw-icons/rio/color/logo-and-text-horizontal.svg
--rw-r--r--   0        0        0     5961 2020-02-02 00:00:00.000000 rio_ui-0.7.2/raw-icons/rio/color/logo-and-text-vertical.svg
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 rio_ui-0.7.2/raw-icons/rio/color/logo.svg
--rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 rio_ui-0.7.2/raw-icons/rio/fill/logo-and-text-horizontal.svg
--rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 rio_ui-0.7.2/raw-icons/rio/fill/logo-and-text-vertical.svg
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 rio_ui-0.7.2/raw-icons/rio/fill/logo.svg
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 rio_ui-0.7.2/raw-icons/styling/corner-round-bottom-left.svg
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 rio_ui-0.7.2/raw-icons/styling/corner-round-bottom-right.svg
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 rio_ui-0.7.2/raw-icons/styling/corner-round-top-left.svg
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 rio_ui-0.7.2/raw-icons/styling/corner-round-top-right.svg
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/__init__.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/__main__.py
--rw-r--r--   0        0        0    19320 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/app.py
--rw-r--r--   0        0        0    32919 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/app_server.py
--rw-r--r--   0        0        0     8672 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/assets.py
--rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/byte_serving.py
--rw-r--r--   0        0        0    19465 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/color.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/cursor_style.py
--rw-r--r--   0        0        0     6033 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/dataclass.py
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/errors.py
--rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/event.py
--rw-r--r--   0        0        0     6690 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/fills.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/global_state.py
--rw-r--r--   0        0        0     9857 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/icon_registry.py
--rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/inspection.py
--rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/maybes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/py.typed
--rw-r--r--   0        0        0     8057 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/routing.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/self_serializing.py
--rw-r--r--   0        0        0     8519 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/serialization.py
--rw-r--r--   0        0        0    79752 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/session.py
--rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/session_attachments.py
--rw-r--r--   0        0        0     8246 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/state_properties.py
--rw-r--r--   0        0        0     4492 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/text_style.py
--rw-r--r--   0        0        0    28614 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/theme.py
--rw-r--r--   0        0        0     5401 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/user_settings_module.py
--rw-r--r--   0        0        0    10026 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/utils.py
--rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/world_units.py
--rw-r--r--   0        0        0    11560 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/assets/fonts/Roboto/LICENSE.txt
--rw-r--r--   0        0        0   167336 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/assets/fonts/Roboto/Roboto-Bold.ttf
--rw-r--r--   0        0        0   171508 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/assets/fonts/Roboto/Roboto-BoldItalic.ttf
--rw-r--r--   0        0        0   170504 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/assets/fonts/Roboto/Roboto-Italic.ttf
--rw-r--r--   0        0        0   168260 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/assets/fonts/Roboto/Roboto-Regular.ttf
--rw-r--r--   0        0        0    11560 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/assets/fonts/Roboto Mono/LICENSE.txt
--rw-r--r--   0        0        0    87392 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/assets/fonts/Roboto Mono/RobotoMono-Bold.ttf
--rw-r--r--   0        0        0    94636 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/assets/fonts/Roboto Mono/RobotoMono-BoldItalic.ttf
--rw-r--r--   0        0        0    94372 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/assets/fonts/Roboto Mono/RobotoMono-Italic.ttf
--rw-r--r--   0        0        0    87236 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/assets/fonts/Roboto Mono/RobotoMono-Regular.ttf
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/assets/hosted/README.md
--rw-r--r--   0        0        0    54189 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/assets/hosted/rio-logos/logo-and-text-horizontal.png
--rw-r--r--   0        0        0    31665 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/assets/hosted/rio-logos/rio-logo-square.png
--rw-r--r--   0        0        0  1081336 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/assets/icon-sets/material.tar.xz
--rw-r--r--   0        0        0    14992 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/assets/icon-sets/rio.tar.xz
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/assets/icon-sets/styling.tar.xz
--rw-r--r--   0        0        0     7375 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/cli/__init__.py
--rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/cli/cli_instance.py
--rw-r--r--   0        0        0     6672 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/cli/nice_traceback.py
--rw-r--r--   0        0        0    14016 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/cli/project.py
--rw-r--r--   0        0        0    14492 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/cli/project_setup.py
--rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/cli/rio_api.py
--rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/cli/rioignore.py
--rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/cli/tomlconfig.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/cli/run_project/__init__.py
--rw-r--r--   0        0        0     5446 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/cli/run_project/app_loading.py
--rw-r--r--   0        0        0    22577 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/cli/run_project/arbiter.py
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/cli/run_project/file_watcher_worker.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/cli/run_project/run_models.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/cli/run_project/run_utils.py
--rw-r--r--   0        0        0     4155 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/cli/run_project/uvicorn_worker.py
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/cli/run_project/webview_worker.py
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/__init__.py
--rw-r--r--   0        0        0     4469 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/app_root.py
--rw-r--r--   0        0        0     4167 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/auto_form.py
--rw-r--r--   0        0        0     4800 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/banner.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/build_failed.py
--rw-r--r--   0        0        0    12739 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/button.py
--rw-r--r--   0        0        0     5325 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/card.py
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/class_container.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/code_block.py
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/code_explorer.py
--rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/color_picker.py
--rw-r--r--   0        0        0    26340 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/component.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/component_tree.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/container.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/debugger_connector.py
--rw-r--r--   0        0        0     4152 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/devel_component.py
--rw-r--r--   0        0        0     4274 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/drawer.py
--rw-r--r--   0        0        0     7070 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/dropdown.py
--rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/flow_container.py
--rw-r--r--   0        0        0     6075 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/fundamental_component.py
--rw-r--r--   0        0        0     7087 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/grid.py
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/html.py
--rw-r--r--   0        0        0     7709 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/icon.py
--rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/image.py
--rw-r--r--   0        0        0    14169 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/key_event_listener.py
--rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/labeled_column.py
--rw-r--r--   0        0        0    10697 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/linear_containers.py
--rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/link.py
--rw-r--r--   0        0        0    10524 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/list_items.py
--rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/list_view.py
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/markdown.py
--rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/media_player.py
--rw-r--r--   0        0        0    10800 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/mouse_event_listener.py
--rw-r--r--   0        0        0     5140 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/multi_line_text_input.py
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/node_input.py
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/node_output.py
--rw-r--r--   0        0        0     9335 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/number_input.py
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/overlay.py
--rw-r--r--   0        0        0     5147 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/page_view.py
--rw-r--r--   0        0        0     4992 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/plot.py
--rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/popup.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/progress_bar.py
--rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/progress_circle.py
--rw-r--r--   0        0        0     5702 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/rectangle.py
--rw-r--r--   0        0        0     4038 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/revealer.py
--rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/root_components.py
--rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/scroll_container.py
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/scroll_target.py
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/separator.py
--rw-r--r--   0        0        0     5947 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/slider.py
--rw-r--r--   0        0        0     3585 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/slideshow.py
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/spacer.py
--rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/stack.py
--rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/switch.py
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/switcher.py
--rw-r--r--   0        0        0     9204 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/switcher_bar.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/table.py
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/text.py
--rw-r--r--   0        0        0     6144 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/text_input.py
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/theme_context_switcher.py
--rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/tooltip.py
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/components/website.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/debug/__init__.py
--rw-r--r--   0        0        0     7485 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/debug/monkeypatches.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/debug/typing_utils.py
--rw-r--r--   0        0        0    14479 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/debug/validator.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/debug/dev_tools/__init__.py
--rw-r--r--   0        0        0    10582 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/debug/dev_tools/component_details.py
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/debug/dev_tools/deploy_page.py
--rw-r--r--   0        0        0     3598 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/debug/dev_tools/dev_tools_sidebar.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/debug/dev_tools/docs_page.py
--rw-r--r--   0        0        0    12890 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/debug/dev_tools/icons_page.py
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/debug/dev_tools/layout_preview.py
--rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/debug/dev_tools/project_page.py
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/debug/dev_tools/sample_icons_grid.py
--rw-r--r--   0        0        0    17346 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/debug/dev_tools/theme_picker_page.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/debug/dev_tools/tree_page.py
--rw-r--r--   0        0        0    10466 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/docs/__init__.py
--rw-r--r--   0        0        0   416487 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/generated/index.html
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/patches_for_3rd_party_stuff/IocpProactor_accept_locals_accept_coro.py
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/patches_for_3rd_party_stuff/ProactorBasePipeTransport_call_connection_lost.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/patches_for_3rd_party_stuff/_OverlappedFuture_cancel_overlapped.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/patches_for_3rd_party_stuff/__init__.py
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/README.md
--rw-r--r--   0        0        0    15602 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/__init__.py
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/howtos/core-classes.md
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/howtos/debugging-setup.md
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/howtos/deployment.md
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/howtos/howto-custom-events.md
--rw-r--r--   0        0        0     5844 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/howtos/howto-get-value-from-child-component.md
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/howtos/howto-install.md
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/howtos/howto-pass-value-to-event.md
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/howtos/persistent-settings.md
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/howtos/project-setup.md
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/howtos/run-project.md
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/howtos/theming.md
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/howtos-todo/attribute-bindings.md
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/howtos-todo/component-lifecycle.md
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/howtos-todo/custom-events.md
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/howtos-todo/force-refresh.md
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/howtos-todo/initialize-component-asynchronously.md
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/howtos-todo/layouting.md
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/howtos-todo/multiple-pages.md
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/other-examples/simple_counter_app.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-AI Chatbot/README.md
--rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-AI Chatbot/conversation.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-AI Chatbot/meta.json
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-AI Chatbot/root_init.py
--rw-r--r--   0        0        0   258496 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-AI Chatbot/thumbnail.svg
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-AI Chatbot/components/__init__.py
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_message.py
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_suggestion_card.py
--rw-r--r--   0        0        0     3728 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-AI Chatbot/components/empty_chat_placeholder.py
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-AI Chatbot/components/generating_response_placeholder.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-AI Chatbot/pages/__init__.py
--rw-r--r--   0        0        0     5823 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-AI Chatbot/pages/chat_page.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Crypto Dashboard/README.md
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Crypto Dashboard/data_models.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Crypto Dashboard/meta.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Crypto Dashboard/root_init.py
--rw-r--r--   0        0        0   270445 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Crypto Dashboard/thumbnail.svg
--rw-r--r--   0        0        0     7595 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Crypto Dashboard/assets/cryptos.csv
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/__init__.py
--rw-r--r--   0        0        0    10704 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/balance_card.py
--rw-r--r--   0        0        0     6695 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_card.py
--rw-r--r--   0        0        0     5604 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_chart.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Crypto Dashboard/pages/__init__.py
--rw-r--r--   0        0        0     7668 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Crypto Dashboard/pages/dashboard_page.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Empty/README.md
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Empty/meta.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Empty/root_init.py
--rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Empty/thumbnail.svg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Empty/pages/__init__.py
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Empty/pages/sample_page.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Multipage Website/README.md
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Multipage Website/meta.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Multipage Website/root_init.py
--rw-r--r--   0        0        0   208005 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Multipage Website/thumbnail.svg
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Multipage Website/components/__init__.py
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Multipage Website/components/footer.py
--rw-r--r--   0        0        0     4826 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Multipage Website/components/navbar.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Multipage Website/components/news_article.py
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Multipage Website/components/testimonial.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Multipage Website/pages/__init__.py
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Multipage Website/pages/about_page.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Multipage Website/pages/home_page.py
--rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Multipage Website/pages/news_page.py
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Multipage Website/pages/root_page.py
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Simple CRUD/README.md
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Simple CRUD/data_models.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Simple CRUD/meta.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Simple CRUD/root_init.py
--rw-r--r--   0        0        0   350009 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Simple CRUD/thumbnail.svg
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Simple CRUD/components/__init__.py
--rw-r--r--   0        0        0     7284 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_editor.py
--rw-r--r--   0        0        0     5810 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_list.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Simple CRUD/pages/__init__.py
--rw-r--r--   0        0        0     8587 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Simple CRUD/pages/crud_page.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/README.md
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/meta.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/root_init.py
--rw-r--r--   0        0        0    23769 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/thumbnail.svg
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/__init__.py
--rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/field.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/__init__.py
--rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/tic_tac_toe_page.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/components/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/__init__.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/tic_tac_toe_page.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/__init__.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/field.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/__init__.py
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/tic_tac_toe_page.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/__init__.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/field.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/__init__.py
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/tic_tac_toe_page.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/__init__.py
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/field.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/__init__.py
--rw-r--r--   0        0        0     4348 2020-02-02 00:00:00.000000 rio_ui-0.7.2/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/tic_tac_toe_page.py
--rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 rio_ui-0.7.2/scripts/benchmark.py
--rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 rio_ui-0.7.2/scripts/build_material_icon_set.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 rio_ui-0.7.2/scripts/cloc.sh
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 rio_ui-0.7.2/scripts/code_coverage.py
--rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 rio_ui-0.7.2/scripts/publish_new_release.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 rio_ui-0.7.2/tests/test_app_build.py
--rw-r--r--   0        0        0     8822 2020-02-02 00:00:00.000000 rio_ui-0.7.2/tests/test_attribute_bindings.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 rio_ui-0.7.2/tests/test_custom_components.py
--rw-r--r--   0        0        0     3426 2020-02-02 00:00:00.000000 rio_ui-0.7.2/tests/test_docstring_code_blocks.py
--rw-r--r--   0        0        0     3797 2020-02-02 00:00:00.000000 rio_ui-0.7.2/tests/test_documentation.py
--rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 rio_ui-0.7.2/tests/test_events.py
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 rio_ui-0.7.2/tests/test_project_templates.py
--rw-r--r--   0        0        0    11737 2020-02-02 00:00:00.000000 rio_ui-0.7.2/tests/test_reconciliation.py
--rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 rio_ui-0.7.2/tests/test_refresh.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 rio_ui-0.7.2/tests/test_session.py
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 rio_ui-0.7.2/tests/test_user_settings.py
--rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 rio_ui-0.7.2/tests/test_zzz_guardrails.py
--rw-r--r--   0        0        0     8596 2020-02-02 00:00:00.000000 rio_ui-0.7.2/tests/utils.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 rio_ui-0.7.2/.gitignore
--rw-r--r--   0        0        0    11315 2020-02-02 00:00:00.000000 rio_ui-0.7.2/LICENSE.txt
--rw-r--r--   0        0        0     7523 2020-02-02 00:00:00.000000 rio_ui-0.7.2/README.md
--rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 rio_ui-0.7.2/pyproject.toml
--rw-r--r--   0        0        0    22744 2020-02-02 00:00:00.000000 rio_ui-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 rio_ui-0.7.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 rio_ui-0.7.3/.prettierrc
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 rio_ui-0.7.3/.sassrc
+-rw-r--r--   0        0        0     5534 2020-02-02 00:00:00.000000 rio_ui-0.7.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 rio_ui-0.7.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 rio_ui-0.7.3/__init__.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 rio_ui-0.7.3/changelog.md
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 rio_ui-0.7.3/debug.log
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 rio_ui-0.7.3/package.json
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 rio_ui-0.7.3/vite.config.js
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 rio_ui-0.7.3/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 rio_ui-0.7.3/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 rio_ui-0.7.3/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/index.html
+-rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/app.ts
+-rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/colorConversion.ts
+-rw-r--r--   0        0        0    20706 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/componentManagement.ts
+-rw-r--r--   0        0        0     5795 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/cssUtils.ts
+-rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/dataModels.ts
+-rw-r--r--   0        0        0     6925 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/designApplication.ts
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/easeFunctions.ts
+-rw-r--r--   0        0        0     4869 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/eventHandling.ts
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/inputBoxTools.ts
+-rw-r--r--   0        0        0     6081 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/layoutHelpers.ts
+-rw-r--r--   0        0        0     4878 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/layouting.ts
+-rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/rippleEffect.ts
+-rw-r--r--   0        0        0    11646 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/rpc.ts
+-rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/rpcFunctions.ts
+-rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/utils.ts
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/components/align.ts
+-rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/components/buildFailed.ts
+-rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/components/button.ts
+-rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/components/card.ts
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/components/classContainer.ts
+-rw-r--r--   0        0        0     6349 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/components/codeBlock.ts
+-rw-r--r--   0        0        0    15146 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/components/codeExplorer.ts
+-rw-r--r--   0        0        0    13820 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/components/colorPicker.ts
+-rw-r--r--   0        0        0    13570 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/components/componentBase.ts
+-rw-r--r--   0        0        0    14334 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/components/componentTree.ts
+-rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/components/customListItem.ts
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/components/debuggerConnector.ts
+-rw-r--r--   0        0        0    11400 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/components/drawer.ts
+-rw-r--r--   0        0        0    16927 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/components/dropdown.ts
+-rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/components/flowContainer.ts
+-rw-r--r--   0        0        0     5700 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/components/fundamentalRootComponent.ts
+-rw-r--r--   0        0        0    11004 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/components/grid.ts
+-rw-r--r--   0        0        0     2201 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/components/headingListItem.ts
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/components/html.ts
+-rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/components/icon.ts
+-rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/components/image.ts
+-rw-r--r--   0        0        0    19839 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/components/keyEventListener.ts
+-rw-r--r--   0        0        0     9923 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/components/linearContainers.ts
+-rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/components/link.ts
+-rw-r--r--   0        0        0     4575 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/components/listView.ts
+-rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/components/margin.ts
+-rw-r--r--   0        0        0     6268 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/components/markdown.ts
+-rw-r--r--   0        0        0    27995 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/components/mediaPlayer.ts
+-rw-r--r--   0        0        0     5948 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/components/mouseEventListener.ts
+-rw-r--r--   0        0        0     4122 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/components/multiLineTextInput.ts
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/components/nodeInput.ts
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/components/nodeOutput.ts
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/components/overlay.ts
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/components/placeholder.ts
+-rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/components/plot.ts
+-rw-r--r--   0        0        0     7055 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/components/popup.ts
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/components/progressBar.ts
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/components/progressCircle.ts
+-rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/components/rectangle.ts
+-rw-r--r--   0        0        0    10840 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/components/revealer.ts
+-rw-r--r--   0        0        0     9454 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/components/scrollContainer.ts
+-rw-r--r--   0        0        0     6620 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/components/scrollTarget.ts
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/components/separator.ts
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/components/separatorListItem.ts
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/components/singleContainer.ts
+-rw-r--r--   0        0        0     5031 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/components/slider.ts
+-rw-r--r--   0        0        0     7104 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/components/slideshow.ts
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/components/stack.ts
+-rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/components/switch.ts
+-rw-r--r--   0        0        0     8056 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/components/switcher.ts
+-rw-r--r--   0        0        0    19999 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/components/switcherBar.ts
+-rw-r--r--   0        0        0     8067 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/components/table.ts
+-rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/components/text.ts
+-rw-r--r--   0        0        0     7311 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/components/textInput.ts
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/components/themeContextSwitcher.ts
+-rw-r--r--   0        0        0     4463 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/components/tooltip.ts
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/code/components/website.ts
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/css/highlightjs-default-dark.css
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/css/highlightjs-default-light.css
+-rw-r--r--   0        0        0    50930 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/css/style.scss
+-rw-r--r--   0        0        0     8244 2020-02-02 00:00:00.000000 rio_ui-0.7.3/frontend/css/switcheroos.scss
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 rio_ui-0.7.3/raw-icons/custom-material-icons/twinkle.svg
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 rio_ui-0.7.3/raw-icons/custom-material-icons/fill/twinkle.svg
+-rw-r--r--   0        0        0    10067 2020-02-02 00:00:00.000000 rio_ui-0.7.3/raw-icons/rio/logo-and-text-horizontal.svg
+-rw-r--r--   0        0        0    10127 2020-02-02 00:00:00.000000 rio_ui-0.7.3/raw-icons/rio/logo-and-text-vertical.svg
+-rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 rio_ui-0.7.3/raw-icons/rio/logo.svg
+-rw-r--r--   0        0        0     5933 2020-02-02 00:00:00.000000 rio_ui-0.7.3/raw-icons/rio/color/logo-and-text-horizontal.svg
+-rw-r--r--   0        0        0     5961 2020-02-02 00:00:00.000000 rio_ui-0.7.3/raw-icons/rio/color/logo-and-text-vertical.svg
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 rio_ui-0.7.3/raw-icons/rio/color/logo.svg
+-rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 rio_ui-0.7.3/raw-icons/rio/fill/logo-and-text-horizontal.svg
+-rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 rio_ui-0.7.3/raw-icons/rio/fill/logo-and-text-vertical.svg
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 rio_ui-0.7.3/raw-icons/rio/fill/logo.svg
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 rio_ui-0.7.3/raw-icons/styling/corner-round-bottom-left.svg
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 rio_ui-0.7.3/raw-icons/styling/corner-round-bottom-right.svg
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 rio_ui-0.7.3/raw-icons/styling/corner-round-top-left.svg
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 rio_ui-0.7.3/raw-icons/styling/corner-round-top-right.svg
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/__init__.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/__main__.py
+-rw-r--r--   0        0        0    19320 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/app.py
+-rw-r--r--   0        0        0    32919 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/app_server.py
+-rw-r--r--   0        0        0     8672 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/assets.py
+-rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/byte_serving.py
+-rw-r--r--   0        0        0    19465 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/color.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/cursor_style.py
+-rw-r--r--   0        0        0     6033 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/dataclass.py
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/errors.py
+-rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/event.py
+-rw-r--r--   0        0        0     6690 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/fills.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/global_state.py
+-rw-r--r--   0        0        0     9857 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/icon_registry.py
+-rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/inspection.py
+-rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/maybes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/py.typed
+-rw-r--r--   0        0        0     8057 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/routing.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/self_serializing.py
+-rw-r--r--   0        0        0     8519 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/serialization.py
+-rw-r--r--   0        0        0    80113 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/session.py
+-rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/session_attachments.py
+-rw-r--r--   0        0        0     8246 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/state_properties.py
+-rw-r--r--   0        0        0     8831 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/testing.py
+-rw-r--r--   0        0        0     4492 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/text_style.py
+-rw-r--r--   0        0        0    28614 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/theme.py
+-rw-r--r--   0        0        0     5832 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/user_settings_module.py
+-rw-r--r--   0        0        0    10338 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/utils.py
+-rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/world_units.py
+-rw-r--r--   0        0        0    11560 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/assets/fonts/Roboto/LICENSE.txt
+-rw-r--r--   0        0        0   167336 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/assets/fonts/Roboto/Roboto-Bold.ttf
+-rw-r--r--   0        0        0   171508 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/assets/fonts/Roboto/Roboto-BoldItalic.ttf
+-rw-r--r--   0        0        0   170504 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/assets/fonts/Roboto/Roboto-Italic.ttf
+-rw-r--r--   0        0        0   168260 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/assets/fonts/Roboto/Roboto-Regular.ttf
+-rw-r--r--   0        0        0    11560 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/assets/fonts/Roboto Mono/LICENSE.txt
+-rw-r--r--   0        0        0    87392 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/assets/fonts/Roboto Mono/RobotoMono-Bold.ttf
+-rw-r--r--   0        0        0    94636 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/assets/fonts/Roboto Mono/RobotoMono-BoldItalic.ttf
+-rw-r--r--   0        0        0    94372 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/assets/fonts/Roboto Mono/RobotoMono-Italic.ttf
+-rw-r--r--   0        0        0    87236 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/assets/fonts/Roboto Mono/RobotoMono-Regular.ttf
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/assets/hosted/README.md
+-rw-r--r--   0        0        0    54189 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/assets/hosted/rio-logos/logo-and-text-horizontal.png
+-rw-r--r--   0        0        0    31665 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/assets/hosted/rio-logos/rio-logo-square.png
+-rw-r--r--   0        0        0  1081336 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/assets/icon-sets/material.tar.xz
+-rw-r--r--   0        0        0    14992 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/assets/icon-sets/rio.tar.xz
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/assets/icon-sets/styling.tar.xz
+-rw-r--r--   0        0        0     7375 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/cli/__init__.py
+-rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/cli/cli_instance.py
+-rw-r--r--   0        0        0     6672 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/cli/nice_traceback.py
+-rw-r--r--   0        0        0    14016 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/cli/project.py
+-rw-r--r--   0        0        0    14492 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/cli/project_setup.py
+-rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/cli/rio_api.py
+-rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/cli/rioignore.py
+-rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/cli/tomlconfig.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/cli/run_project/__init__.py
+-rw-r--r--   0        0        0     5446 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/cli/run_project/app_loading.py
+-rw-r--r--   0        0        0    22577 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/cli/run_project/arbiter.py
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/cli/run_project/file_watcher_worker.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/cli/run_project/run_models.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/cli/run_project/run_utils.py
+-rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/cli/run_project/uvicorn_worker.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/cli/run_project/webview_worker.py
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/__init__.py
+-rw-r--r--   0        0        0     4469 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/app_root.py
+-rw-r--r--   0        0        0     4167 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/auto_form.py
+-rw-r--r--   0        0        0     4800 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/banner.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/build_failed.py
+-rw-r--r--   0        0        0    12732 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/button.py
+-rw-r--r--   0        0        0     5325 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/card.py
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/class_container.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/code_block.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/code_explorer.py
+-rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/color_picker.py
+-rw-r--r--   0        0        0    26340 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/component.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/component_tree.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/container.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/debugger_connector.py
+-rw-r--r--   0        0        0     4152 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/devel_component.py
+-rw-r--r--   0        0        0     4274 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/drawer.py
+-rw-r--r--   0        0        0     7070 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/dropdown.py
+-rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/flow_container.py
+-rw-r--r--   0        0        0     6075 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/fundamental_component.py
+-rw-r--r--   0        0        0     7087 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/grid.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/html.py
+-rw-r--r--   0        0        0     7709 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/icon.py
+-rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/image.py
+-rw-r--r--   0        0        0    14169 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/key_event_listener.py
+-rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/labeled_column.py
+-rw-r--r--   0        0        0    10697 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/linear_containers.py
+-rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/link.py
+-rw-r--r--   0        0        0    10571 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/list_items.py
+-rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/list_view.py
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/markdown.py
+-rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/media_player.py
+-rw-r--r--   0        0        0    10800 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/mouse_event_listener.py
+-rw-r--r--   0        0        0     5140 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/multi_line_text_input.py
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/node_input.py
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/node_output.py
+-rw-r--r--   0        0        0     9335 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/number_input.py
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/overlay.py
+-rw-r--r--   0        0        0     5147 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/page_view.py
+-rw-r--r--   0        0        0     4992 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/plot.py
+-rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/popup.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/progress_bar.py
+-rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/progress_circle.py
+-rw-r--r--   0        0        0     5702 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/rectangle.py
+-rw-r--r--   0        0        0     4038 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/revealer.py
+-rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/root_components.py
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/scroll_container.py
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/scroll_target.py
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/separator.py
+-rw-r--r--   0        0        0     5947 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/slider.py
+-rw-r--r--   0        0        0     3585 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/slideshow.py
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/spacer.py
+-rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/stack.py
+-rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/switch.py
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/switcher.py
+-rw-r--r--   0        0        0     9204 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/switcher_bar.py
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/table.py
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/text.py
+-rw-r--r--   0        0        0     6144 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/text_input.py
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/theme_context_switcher.py
+-rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/tooltip.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/components/website.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/debug/__init__.py
+-rw-r--r--   0        0        0     7485 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/debug/monkeypatches.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/debug/typing_utils.py
+-rw-r--r--   0        0        0    14479 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/debug/validator.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/debug/dev_tools/__init__.py
+-rw-r--r--   0        0        0    10582 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/debug/dev_tools/component_details.py
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/debug/dev_tools/deploy_page.py
+-rw-r--r--   0        0        0     3598 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/debug/dev_tools/dev_tools_sidebar.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/debug/dev_tools/docs_page.py
+-rw-r--r--   0        0        0    12890 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/debug/dev_tools/icons_page.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/debug/dev_tools/layout_preview.py
+-rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/debug/dev_tools/project_page.py
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/debug/dev_tools/sample_icons_grid.py
+-rw-r--r--   0        0        0    17346 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/debug/dev_tools/theme_picker_page.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/debug/dev_tools/tree_page.py
+-rw-r--r--   0        0        0    10466 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/docs/__init__.py
+-rw-r--r--   0        0        0   416487 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/generated/index.html
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/patches_for_3rd_party_stuff/IocpProactor_accept_locals_accept_coro.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/patches_for_3rd_party_stuff/ProactorBasePipeTransport_call_connection_lost.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/patches_for_3rd_party_stuff/_OverlappedFuture_cancel_overlapped.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/patches_for_3rd_party_stuff/__init__.py
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/README.md
+-rw-r--r--   0        0        0    15618 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/__init__.py
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/howtos/core-classes.md
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/howtos/debugging-setup.md
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/howtos/deployment.md
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/howtos/howto-custom-events.md
+-rw-r--r--   0        0        0     5844 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/howtos/howto-get-value-from-child-component.md
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/howtos/howto-install.md
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/howtos/howto-pass-value-to-event.md
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/howtos/persistent-settings.md
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/howtos/project-setup.md
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/howtos/run-project.md
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/howtos/theming.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/howtos-todo/attribute-bindings.md
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/howtos-todo/component-lifecycle.md
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/howtos-todo/custom-events.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/howtos-todo/force-refresh.md
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/howtos-todo/initialize-component-asynchronously.md
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/howtos-todo/layouting.md
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/howtos-todo/multiple-pages.md
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/other-examples/simple_counter_app.py
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-AI Chatbot/README.md
+-rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-AI Chatbot/conversation.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-AI Chatbot/meta.json
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-AI Chatbot/root_init.py
+-rw-r--r--   0        0        0   258496 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-AI Chatbot/thumbnail.svg
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-AI Chatbot/components/__init__.py
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_message.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_suggestion_card.py
+-rw-r--r--   0        0        0     3728 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-AI Chatbot/components/empty_chat_placeholder.py
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-AI Chatbot/components/generating_response_placeholder.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-AI Chatbot/pages/__init__.py
+-rw-r--r--   0        0        0     5823 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-AI Chatbot/pages/chat_page.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Crypto Dashboard/README.md
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Crypto Dashboard/data_models.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Crypto Dashboard/meta.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Crypto Dashboard/root_init.py
+-rw-r--r--   0        0        0   270445 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Crypto Dashboard/thumbnail.svg
+-rw-r--r--   0        0        0     7595 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Crypto Dashboard/assets/cryptos.csv
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/__init__.py
+-rw-r--r--   0        0        0    10704 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/balance_card.py
+-rw-r--r--   0        0        0     6695 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_card.py
+-rw-r--r--   0        0        0     5604 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_chart.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Crypto Dashboard/pages/__init__.py
+-rw-r--r--   0        0        0     7668 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Crypto Dashboard/pages/dashboard_page.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Empty/README.md
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Empty/meta.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Empty/root_init.py
+-rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Empty/thumbnail.svg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Empty/pages/__init__.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Empty/pages/sample_page.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Multipage Website/README.md
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Multipage Website/meta.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Multipage Website/root_init.py
+-rw-r--r--   0        0        0   208005 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Multipage Website/thumbnail.svg
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Multipage Website/components/__init__.py
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Multipage Website/components/footer.py
+-rw-r--r--   0        0        0     4826 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Multipage Website/components/navbar.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Multipage Website/components/news_article.py
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Multipage Website/components/testimonial.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Multipage Website/pages/__init__.py
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Multipage Website/pages/about_page.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Multipage Website/pages/home_page.py
+-rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Multipage Website/pages/news_page.py
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Multipage Website/pages/root_page.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Simple CRUD/README.md
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Simple CRUD/data_models.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Simple CRUD/meta.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Simple CRUD/root_init.py
+-rw-r--r--   0        0        0   350009 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Simple CRUD/thumbnail.svg
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Simple CRUD/components/__init__.py
+-rw-r--r--   0        0        0     7284 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_editor.py
+-rw-r--r--   0        0        0     5810 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_list.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Simple CRUD/pages/__init__.py
+-rw-r--r--   0        0        0     8587 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Simple CRUD/pages/crud_page.py
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/README.md
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/meta.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/root_init.py
+-rw-r--r--   0        0        0    23769 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/thumbnail.svg
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/__init__.py
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/field.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/__init__.py
+-rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/tic_tac_toe_page.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Todo App/README.md
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Todo App/data_models.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Todo App/meta.json
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Todo App/root_init.py
+-rw-r--r--   0        0        0   117987 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Todo App/thumbnail.svg
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Todo App/components/__init__.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Todo App/components/new_todo_item_input.py
+-rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Todo App/components/todo_item_component.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Todo App/pages/__init__.py
+-rw-r--r--   0        0        0     3119 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Todo App/pages/todo_list_page.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/components/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/__init__.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/tic_tac_toe_page.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/__init__.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/field.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/__init__.py
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/tic_tac_toe_page.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/__init__.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/field.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/__init__.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/tic_tac_toe_page.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/__init__.py
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/field.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/__init__.py
+-rw-r--r--   0        0        0     4348 2020-02-02 00:00:00.000000 rio_ui-0.7.3/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/tic_tac_toe_page.py
+-rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 rio_ui-0.7.3/scripts/benchmark.py
+-rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 rio_ui-0.7.3/scripts/build_material_icon_set.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 rio_ui-0.7.3/scripts/cloc.sh
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 rio_ui-0.7.3/scripts/code_coverage.py
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 rio_ui-0.7.3/scripts/publish_new_release.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 rio_ui-0.7.3/tests/test_app_build.py
+-rw-r--r--   0        0        0     9804 2020-02-02 00:00:00.000000 rio_ui-0.7.3/tests/test_attribute_bindings.py
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 rio_ui-0.7.3/tests/test_custom_components.py
+-rw-r--r--   0        0        0     3748 2020-02-02 00:00:00.000000 rio_ui-0.7.3/tests/test_docstring_code_blocks.py
+-rw-r--r--   0        0        0     3797 2020-02-02 00:00:00.000000 rio_ui-0.7.3/tests/test_documentation.py
+-rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 rio_ui-0.7.3/tests/test_events.py
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 rio_ui-0.7.3/tests/test_project_templates.py
+-rw-r--r--   0        0        0    12411 2020-02-02 00:00:00.000000 rio_ui-0.7.3/tests/test_reconciliation.py
+-rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 rio_ui-0.7.3/tests/test_refresh.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 rio_ui-0.7.3/tests/test_session.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 rio_ui-0.7.3/tests/test_testing_tools.py
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 rio_ui-0.7.3/tests/test_user_settings.py
+-rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 rio_ui-0.7.3/tests/test_zzz_guardrails.py
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 rio_ui-0.7.3/tests/utils.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 rio_ui-0.7.3/.gitignore
+-rw-r--r--   0        0        0    11315 2020-02-02 00:00:00.000000 rio_ui-0.7.3/LICENSE.txt
+-rw-r--r--   0        0        0     7523 2020-02-02 00:00:00.000000 rio_ui-0.7.3/README.md
+-rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 rio_ui-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0    22714 2020-02-02 00:00:00.000000 rio_ui-0.7.3/PKG-INFO
```

### Comparing `rio_ui-0.7.2/CODE_OF_CONDUCT.md` & `rio_ui-0.7.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/CONTRIBUTING.md` & `rio_ui-0.7.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/package.json` & `rio_ui-0.7.3/package.json`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/.github/ISSUE_TEMPLATE/bug_report.yml` & `rio_ui-0.7.3/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     - type: markdown
       attributes:
           value: |
               Thank you for your time to report a bug to the Rio project.
     - type: markdown
       attributes:
           value: |
-              Before filing a new issue, **please do a quick search** to check that it hasn't already been filed on the issue tracker. You can do this by going to [this link](https://github.com/rio-labs/rio/issues) and typing some words related to the issue in the search box next to the "New issue" button.
+              Before submitting a new issue, **please do a quick search** to ensure it hasn't already been raised in the issue tracker. You can do this by going to [this link](https://github.com/rio-labs/rio/issues) and typing some words related to the issue in the search box next to the "New issue" button.
     - type: textarea
       attributes:
           label: Describe the bug
           description: 'A concise description of the issue you''re experiencing. **Example:** "NumberInput is parsing negative numbers incorrectly. When I use -100 as input, the value is correctly processed as -100, but the displayed value is -.100."'
       validations:
           required: true
     - type: textarea
@@ -84,29 +84,17 @@
           label: What device are you using?
           description: Please select the device you're using.
           multiple: true
           options:
               - Desktop
               - Mobile
       validations:
-          required: true
+          required: false
     - type: textarea
       attributes:
           label: Additional context
           description: |
               Add any other context about the problem here.
 
               Tip: You can attach images or log files by clicking this area to highlight it and then dragging files in.
       validations:
           required: false
-    - type: textarea
-      attributes:
-          label: Tips for developers
-          description: Please leave this section as-is.
-          value: |
-              Before addressing the bug, please identify which PR caused the issue (you can follow the steps. If you identify the PR, comment on the issue with a link to it. If not, mention the commit hash of the oldest commit you saw the bug on (and the month and year it was made in).
-
-              Then, please leave a comment with details of the approach that you plan to take to fix the issue.
-
-              **Note:** If this is your first Rio issue, please make sure to follow our [contribution guidelines](https://github.com/rio-labs/rio/blob/68e9193489adbb8378667e8b682b501e962f3eb1/CONTRIBUTING.md#L4). You will also need to show a demo of the fix working correctly on your local machine. Thanks!
-      validations:
-          required: true
```

### Comparing `rio_ui-0.7.2/frontend/index.html` & `rio_ui-0.7.3/frontend/index.html`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/app.ts` & `rio_ui-0.7.3/frontend/code/app.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/colorConversion.ts` & `rio_ui-0.7.3/frontend/code/colorConversion.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/componentManagement.ts` & `rio_ui-0.7.3/frontend/code/componentManagement.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/cssUtils.ts` & `rio_ui-0.7.3/frontend/code/cssUtils.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/dataModels.ts` & `rio_ui-0.7.3/frontend/code/dataModels.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/designApplication.ts` & `rio_ui-0.7.3/frontend/code/designApplication.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/easeFunctions.ts` & `rio_ui-0.7.3/frontend/code/easeFunctions.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/eventHandling.ts` & `rio_ui-0.7.3/frontend/code/eventHandling.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/inputBoxTools.ts` & `rio_ui-0.7.3/frontend/code/inputBoxTools.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/layoutHelpers.ts` & `rio_ui-0.7.3/frontend/code/layoutHelpers.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/layouting.ts` & `rio_ui-0.7.3/frontend/code/layouting.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/rippleEffect.ts` & `rio_ui-0.7.3/frontend/code/rippleEffect.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/rpc.ts` & `rio_ui-0.7.3/frontend/code/rpc.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/rpcFunctions.ts` & `rio_ui-0.7.3/frontend/code/rpcFunctions.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/utils.ts` & `rio_ui-0.7.3/frontend/code/utils.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/components/align.ts` & `rio_ui-0.7.3/frontend/code/components/align.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/components/buildFailed.ts` & `rio_ui-0.7.3/frontend/code/components/buildFailed.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/components/button.ts` & `rio_ui-0.7.3/frontend/code/components/button.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/components/card.ts` & `rio_ui-0.7.3/frontend/code/components/card.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/components/classContainer.ts` & `rio_ui-0.7.3/frontend/code/components/classContainer.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/components/codeBlock.ts` & `rio_ui-0.7.3/frontend/code/components/codeBlock.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/components/codeExplorer.ts` & `rio_ui-0.7.3/frontend/code/components/codeExplorer.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/components/colorPicker.ts` & `rio_ui-0.7.3/frontend/code/components/colorPicker.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/components/componentBase.ts` & `rio_ui-0.7.3/frontend/code/components/componentBase.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/components/componentTree.ts` & `rio_ui-0.7.3/frontend/code/components/componentTree.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/components/customListItem.ts` & `rio_ui-0.7.3/frontend/code/components/customListItem.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/components/debuggerConnector.ts` & `rio_ui-0.7.3/frontend/code/components/debuggerConnector.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/components/drawer.ts` & `rio_ui-0.7.3/frontend/code/components/drawer.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/components/dropdown.ts` & `rio_ui-0.7.3/frontend/code/components/dropdown.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/components/flowContainer.ts` & `rio_ui-0.7.3/frontend/code/components/flowContainer.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/components/fundamentalRootComponent.ts` & `rio_ui-0.7.3/frontend/code/components/fundamentalRootComponent.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/components/grid.ts` & `rio_ui-0.7.3/frontend/code/components/grid.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/components/headingListItem.ts` & `rio_ui-0.7.3/frontend/code/components/headingListItem.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/components/html.ts` & `rio_ui-0.7.3/frontend/code/components/html.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/components/icon.ts` & `rio_ui-0.7.3/frontend/code/components/icon.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/components/image.ts` & `rio_ui-0.7.3/frontend/code/components/image.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/components/keyEventListener.ts` & `rio_ui-0.7.3/frontend/code/components/keyEventListener.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/components/linearContainers.ts` & `rio_ui-0.7.3/frontend/code/components/linearContainers.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/components/link.ts` & `rio_ui-0.7.3/frontend/code/components/link.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/components/listView.ts` & `rio_ui-0.7.3/frontend/code/components/listView.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/components/margin.ts` & `rio_ui-0.7.3/frontend/code/components/margin.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/components/markdown.ts` & `rio_ui-0.7.3/frontend/code/components/markdown.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/components/mediaPlayer.ts` & `rio_ui-0.7.3/frontend/code/components/mediaPlayer.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/components/mouseEventListener.ts` & `rio_ui-0.7.3/frontend/code/components/mouseEventListener.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/components/multiLineTextInput.ts` & `rio_ui-0.7.3/frontend/code/components/multiLineTextInput.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/components/nodeInput.ts` & `rio_ui-0.7.3/frontend/code/components/nodeInput.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/components/nodeOutput.ts` & `rio_ui-0.7.3/frontend/code/components/nodeOutput.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/components/overlay.ts` & `rio_ui-0.7.3/frontend/code/components/overlay.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/components/placeholder.ts` & `rio_ui-0.7.3/frontend/code/components/placeholder.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/components/plot.ts` & `rio_ui-0.7.3/frontend/code/components/plot.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/components/popup.ts` & `rio_ui-0.7.3/frontend/code/components/popup.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/components/progressBar.ts` & `rio_ui-0.7.3/frontend/code/components/progressBar.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/components/progressCircle.ts` & `rio_ui-0.7.3/frontend/code/components/progressCircle.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/components/rectangle.ts` & `rio_ui-0.7.3/frontend/code/components/rectangle.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/components/revealer.ts` & `rio_ui-0.7.3/frontend/code/components/revealer.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/components/scrollContainer.ts` & `rio_ui-0.7.3/frontend/code/components/scrollContainer.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/components/scrollTarget.ts` & `rio_ui-0.7.3/frontend/code/components/scrollTarget.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/components/separator.ts` & `rio_ui-0.7.3/frontend/code/components/separator.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/components/separatorListItem.ts` & `rio_ui-0.7.3/frontend/code/components/separatorListItem.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/components/singleContainer.ts` & `rio_ui-0.7.3/frontend/code/components/singleContainer.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/components/slider.ts` & `rio_ui-0.7.3/frontend/code/components/slider.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/components/slideshow.ts` & `rio_ui-0.7.3/frontend/code/components/slideshow.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/components/stack.ts` & `rio_ui-0.7.3/frontend/code/components/stack.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/components/switch.ts` & `rio_ui-0.7.3/frontend/code/components/switch.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/components/switcher.ts` & `rio_ui-0.7.3/frontend/code/components/switcher.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/components/switcherBar.ts` & `rio_ui-0.7.3/frontend/code/components/switcherBar.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/components/table.ts` & `rio_ui-0.7.3/frontend/code/components/table.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/components/text.ts` & `rio_ui-0.7.3/frontend/code/components/text.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/components/textInput.ts` & `rio_ui-0.7.3/frontend/code/components/textInput.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/components/themeContextSwitcher.ts` & `rio_ui-0.7.3/frontend/code/components/themeContextSwitcher.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/components/tooltip.ts` & `rio_ui-0.7.3/frontend/code/components/tooltip.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/code/components/website.ts` & `rio_ui-0.7.3/frontend/code/components/website.ts`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/css/highlightjs-default-dark.css` & `rio_ui-0.7.3/frontend/css/highlightjs-default-dark.css`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/css/highlightjs-default-light.css` & `rio_ui-0.7.3/frontend/css/highlightjs-default-light.css`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/css/style.scss` & `rio_ui-0.7.3/frontend/css/style.scss`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/frontend/css/switcheroos.scss` & `rio_ui-0.7.3/frontend/css/switcheroos.scss`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/raw-icons/custom-material-icons/twinkle.svg` & `rio_ui-0.7.3/raw-icons/custom-material-icons/twinkle.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/raw-icons/custom-material-icons/fill/twinkle.svg` & `rio_ui-0.7.3/raw-icons/custom-material-icons/fill/twinkle.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/raw-icons/rio/logo-and-text-horizontal.svg` & `rio_ui-0.7.3/raw-icons/rio/logo-and-text-horizontal.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/raw-icons/rio/logo-and-text-vertical.svg` & `rio_ui-0.7.3/raw-icons/rio/logo-and-text-vertical.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/raw-icons/rio/logo.svg` & `rio_ui-0.7.3/raw-icons/rio/logo.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/raw-icons/rio/color/logo-and-text-horizontal.svg` & `rio_ui-0.7.3/raw-icons/rio/color/logo-and-text-horizontal.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/raw-icons/rio/color/logo-and-text-vertical.svg` & `rio_ui-0.7.3/raw-icons/rio/color/logo-and-text-vertical.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/raw-icons/rio/color/logo.svg` & `rio_ui-0.7.3/raw-icons/rio/color/logo.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/raw-icons/rio/fill/logo-and-text-horizontal.svg` & `rio_ui-0.7.3/raw-icons/rio/fill/logo-and-text-horizontal.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/raw-icons/rio/fill/logo-and-text-vertical.svg` & `rio_ui-0.7.3/raw-icons/rio/fill/logo-and-text-vertical.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/raw-icons/rio/fill/logo.svg` & `rio_ui-0.7.3/raw-icons/rio/fill/logo.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/raw-icons/styling/corner-round-bottom-left.svg` & `rio_ui-0.7.3/raw-icons/styling/corner-round-bottom-left.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/raw-icons/styling/corner-round-bottom-right.svg` & `rio_ui-0.7.3/raw-icons/styling/corner-round-bottom-right.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/raw-icons/styling/corner-round-top-left.svg` & `rio_ui-0.7.3/raw-icons/styling/corner-round-top-left.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/raw-icons/styling/corner-round-top-right.svg` & `rio_ui-0.7.3/raw-icons/styling/corner-round-top-right.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/__init__.py` & `rio_ui-0.7.3/rio/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.7.2"
+__version__ = "0.7.3"
 
 import logging
 
 _logger = logging.getLogger(__name__)
 
 # Re-export dataclass stuff for easy use.
 from dataclasses import KW_ONLY as KW_ONLY
```

### Comparing `rio_ui-0.7.2/rio/app.py` & `rio_ui-0.7.3/rio/app.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/app_server.py` & `rio_ui-0.7.3/rio/app_server.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/assets.py` & `rio_ui-0.7.3/rio/assets.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/byte_serving.py` & `rio_ui-0.7.3/rio/byte_serving.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/color.py` & `rio_ui-0.7.3/rio/color.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/dataclass.py` & `rio_ui-0.7.3/rio/dataclass.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/errors.py` & `rio_ui-0.7.3/rio/errors.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/event.py` & `rio_ui-0.7.3/rio/event.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/fills.py` & `rio_ui-0.7.3/rio/fills.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/global_state.py` & `rio_ui-0.7.3/rio/global_state.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/icon_registry.py` & `rio_ui-0.7.3/rio/icon_registry.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/inspection.py` & `rio_ui-0.7.3/rio/inspection.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/maybes.py` & `rio_ui-0.7.3/rio/maybes.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/routing.py` & `rio_ui-0.7.3/rio/routing.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/serialization.py` & `rio_ui-0.7.3/rio/serialization.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/session.py` & `rio_ui-0.7.3/rio/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,14 +181,19 @@
         # changed.
         self._settings_json_string: str | None = None
 
         # If `running_in_window`, this is the timestamp of when the settings
         # were last saved.
         self._last_settings_save_time: float = -float("inf")
 
+        # A dict of {build_function: BuildFailedComponent}. This is cleared at
+        # the start of every refresh, and tracks which build functions failed.
+        # Used for unit testing.
+        self._crashed_build_functions = dict[Callable, str]()
+
         # Weak dictionaries to hold additional information about components.
         # These are split in two to avoid the dictionaries keeping the
         # components alive. Notice how both dictionaries are weak on the actual
         # component.
         #
         # Never access these directly. Instead, use helper functions
         # - `lookup_component`
@@ -869,14 +874,17 @@
         Afterwards, the client is also informed of any changes, meaning that
         after this method returns there are no more dirty components in the
         session, and Python's state and the client's state are in sync.
         """
 
         # For why this lock is here see its creation in `__init__`
         async with self._refresh_lock:
+            # Clear the dict of crashed build functions
+            self._crashed_build_functions.clear()
+
             while self._dirty_components:
                 # Refresh and get a set of all components which have been visited
                 (
                     visited_components,
                     all_children_old,
                     all_children_new,
                 ) = self._refresh_sync()
```

### Comparing `rio_ui-0.7.2/rio/session_attachments.py` & `rio_ui-0.7.3/rio/session_attachments.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/state_properties.py` & `rio_ui-0.7.3/rio/state_properties.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/text_style.py` & `rio_ui-0.7.3/rio/text_style.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/theme.py` & `rio_ui-0.7.3/rio/theme.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/user_settings_module.py` & `rio_ui-0.7.3/rio/user_settings_module.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import copy
 from dataclasses import field
 from typing import *  # type: ignore
 
 import uniserde
 from typing_extensions import Self
 
-from .dataclass import RioDataclassMeta
+from .dataclass import RioDataclassMeta, all_class_fields
 from . import inspection, session
 
 __all__ = [
     "UserSettings",
 ]
 
 
@@ -157,7 +157,21 @@
 
         # Make sure a write back task is running
         # if self._rio_session_ is not None:
         #     self._rio_session_._save_settings_soon()
 
     if not TYPE_CHECKING:
         __setattr__ = __setattr
+
+    def _equals(self, other: Self) -> bool:
+        if type(self) != type(other):
+            return False
+
+        fields_to_compare = (
+            all_class_fields(type(self)).keys()
+            - all_class_fields(__class__).keys()
+        )
+        for field_name in fields_to_compare:
+            if getattr(self, field_name) != getattr(other, field_name):
+                return False
+
+        return True
```

### Comparing `rio_ui-0.7.2/rio/utils.py` & `rio_ui-0.7.3/rio/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -329,28 +329,37 @@
         rio._logger.exception(
             f"An exception occurred in `{build_function_repr}`"
         )
 
         # Screw circular imports
         from rio.components.build_failed import BuildFailed
 
-        return BuildFailed(f"`{build_function_repr}` has crashed", repr(err))
+        build_failed_component = BuildFailed(
+            f"`{build_function_repr}` has crashed", repr(err)
+        )
+    else:
+        # Make sure the result meets expectations
+        if isinstance(build_result, rio.Component):  # type: ignore (unnecessary isinstance)
+            # All is well
+            return build_result
 
-    # Make sure the result meets expectations
-    if not isinstance(build_result, rio.Component):  # type: ignore (unnecessary isinstance)
         build_function_repr = _repr_build_function(build_function)
 
         rio._logger.error(
             f"The output of `build` methods must be instances of"
             f" `rio.Component`, but `{build_function_repr}` returned `{build_result!r}`"
         )
 
         # Screw circular imports
         from rio.components.build_failed import BuildFailed
 
-        return BuildFailed(
+        build_failed_component = BuildFailed(
             f"`{build_function_repr}` has returned an invalid result",
             f"Build functions must return instances of `rio.Component`, but the result was {build_result!r}",
         )
 
-    # All is well
-    return build_result
+    # Save the error in the session, for testing purposes
+    build_failed_component.session._crashed_build_functions[build_function] = (
+        build_failed_component.error_details
+    )
+
+    return build_failed_component
```

### Comparing `rio_ui-0.7.2/rio/world_units.py` & `rio_ui-0.7.3/rio/world_units.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/assets/fonts/Roboto/LICENSE.txt` & `rio_ui-0.7.3/rio/assets/fonts/Roboto/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/assets/fonts/Roboto/Roboto-Bold.ttf` & `rio_ui-0.7.3/rio/assets/fonts/Roboto/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/assets/fonts/Roboto/Roboto-BoldItalic.ttf` & `rio_ui-0.7.3/rio/assets/fonts/Roboto/Roboto-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/assets/fonts/Roboto/Roboto-Italic.ttf` & `rio_ui-0.7.3/rio/assets/fonts/Roboto/Roboto-Italic.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/assets/fonts/Roboto/Roboto-Regular.ttf` & `rio_ui-0.7.3/rio/assets/fonts/Roboto/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/assets/fonts/Roboto Mono/LICENSE.txt` & `rio_ui-0.7.3/rio/assets/fonts/Roboto Mono/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/assets/fonts/Roboto Mono/RobotoMono-Bold.ttf` & `rio_ui-0.7.3/rio/assets/fonts/Roboto Mono/RobotoMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/assets/fonts/Roboto Mono/RobotoMono-BoldItalic.ttf` & `rio_ui-0.7.3/rio/assets/fonts/Roboto Mono/RobotoMono-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/assets/fonts/Roboto Mono/RobotoMono-Italic.ttf` & `rio_ui-0.7.3/rio/assets/fonts/Roboto Mono/RobotoMono-Italic.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/assets/fonts/Roboto Mono/RobotoMono-Regular.ttf` & `rio_ui-0.7.3/rio/assets/fonts/Roboto Mono/RobotoMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/assets/hosted/rio-logos/logo-and-text-horizontal.png` & `rio_ui-0.7.3/rio/assets/hosted/rio-logos/logo-and-text-horizontal.png`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/assets/hosted/rio-logos/rio-logo-square.png` & `rio_ui-0.7.3/rio/assets/hosted/rio-logos/rio-logo-square.png`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/assets/icon-sets/material.tar.xz` & `rio_ui-0.7.3/rio/assets/icon-sets/material.tar.xz`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/assets/icon-sets/rio.tar.xz` & `rio_ui-0.7.3/rio/assets/icon-sets/rio.tar.xz`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/assets/icon-sets/styling.tar.xz` & `rio_ui-0.7.3/rio/assets/icon-sets/styling.tar.xz`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/cli/__init__.py` & `rio_ui-0.7.3/rio/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/cli/cli_instance.py` & `rio_ui-0.7.3/rio/cli/cli_instance.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/cli/nice_traceback.py` & `rio_ui-0.7.3/rio/cli/nice_traceback.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/cli/project.py` & `rio_ui-0.7.3/rio/cli/project.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/cli/project_setup.py` & `rio_ui-0.7.3/rio/cli/project_setup.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/cli/rio_api.py` & `rio_ui-0.7.3/rio/cli/rio_api.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/cli/rioignore.py` & `rio_ui-0.7.3/rio/cli/rioignore.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/cli/tomlconfig.py` & `rio_ui-0.7.3/rio/cli/tomlconfig.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/cli/run_project/app_loading.py` & `rio_ui-0.7.3/rio/cli/run_project/app_loading.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/cli/run_project/arbiter.py` & `rio_ui-0.7.3/rio/cli/run_project/arbiter.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/cli/run_project/file_watcher_worker.py` & `rio_ui-0.7.3/rio/cli/run_project/file_watcher_worker.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/cli/run_project/uvicorn_worker.py` & `rio_ui-0.7.3/rio/cli/run_project/uvicorn_worker.py`

 * *Files 8% similar despite different names*

```diff
@@ -70,28 +70,14 @@
         serve_task = asyncio.create_task(
             self._uvicorn_server.serve(
                 sockets=[self.socket],
             ),
             name="uvicorn serve",
         )
 
-        # Uvicorn doesn't handle CancelledError properly, which results in ugly
-        # output in the console. This monkeypatch suppresses that.
-        original_receive = uvicorn.lifespan.on.LifespanOn.receive
-
-        async def patched_receive(self) -> Any:
-            try:
-                return await original_receive(self)
-            except asyncio.CancelledError:
-                return {
-                    "type": "lifespan.shutdown",
-                }
-
-        uvicorn.lifespan.on.LifespanOn.receive = patched_receive
-
         # Run the server
         try:
             await asyncio.shield(serve_task)
         except asyncio.CancelledError:
             pass
         except Exception as err:
             rio.cli._logger.exception(f"Uvicorn has crashed")
```

### Comparing `rio_ui-0.7.2/rio/cli/run_project/webview_worker.py` & `rio_ui-0.7.3/rio/cli/run_project/webview_worker.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/components/__init__.py` & `rio_ui-0.7.3/rio/components/__init__.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/components/app_root.py` & `rio_ui-0.7.3/rio/components/app_root.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/components/auto_form.py` & `rio_ui-0.7.3/rio/components/auto_form.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/components/banner.py` & `rio_ui-0.7.3/rio/components/banner.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/components/build_failed.py` & `rio_ui-0.7.3/rio/components/build_failed.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/components/button.py` & `rio_ui-0.7.3/rio/components/button.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         def _on_button_press(self) -> None:
             self.clicks += 1
 
         def build(self) -> rio.Component:
             return rio.Button(
                 rio.Column(
                     rio.Text("Click repeatedly to fill up the progress bar"),
-                    rio.ProgressBar(self.clicks/10, width=15, height=1),
+                    rio.ProgressBar(self.clicks / 10, width=15, height=1),
                 ),
                 on_press=self._on_button_press,
             )
     ```
     """
 
     content: str | rio.Component = ""
@@ -269,30 +269,30 @@
         def build(self) -> rio.Component:
             return rio.IconButton(
                 icon="material/castle",
                 on_press=self.on_press_button,
             )
     ```
 
-    `IconButton`s are commonly used to trigger actions. You can easily achieve this by
-    adding a function call to `on_press`. You can use a function call to update
-    the banner text signaling that the button was pressed:
+    `IconButton`s are commonly used to trigger actions. You can easily achieve
+    this by adding a function call to `on_press`. You can use a function call to
+    update the banner text signaling that the button was pressed:
 
     ```python
     class MyComponent(rio.Component):
         banner_text: str = ""
 
         def on_press_button(self) -> None:
             self.banner_text = "Icon button pressed!"
 
         def build(self) -> rio.Component:
             return rio.Column(
                 rio.Banner(
                     text=self.banner_text,
-                    style="material/info",
+                    style="info",
                 ),
                 rio.IconButton(
                     icon="material/castle",
                     on_press=self.on_press_button,
                 ),
                 spacing=1,
             )
```

### Comparing `rio_ui-0.7.2/rio/components/card.py` & `rio_ui-0.7.3/rio/components/card.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/components/class_container.py` & `rio_ui-0.7.3/rio/components/class_container.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/components/code_block.py` & `rio_ui-0.7.3/rio/components/code_block.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/components/color_picker.py` & `rio_ui-0.7.3/rio/components/color_picker.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     ## Examples
 
     This small example will print a message whenever the user changes the
     selected color:
 
     ```python
     def print_selected_color(event: rio.ColorChangeEvent):
-        print('You selected the color', event.color)
+        print("You selected the color", event.color)
 
     rio.ColorPicker(
         rio.Color.from_hex("#ff0000"),
         on_change=print_selected_color,
     )
     ```
 
@@ -80,17 +80,17 @@
 
         def build(self) -> rio.Component:
             return rio.Row(
                 rio.ColorPicker(
                     color=self.bind().color,
                 ),
                 rio.Icon(
-                    'material/star',
+                    "material/star",
                     fill=self.color,
-                )
+                ),
             )
     ```
     """
 
     color: rio.Color
     _: KW_ONLY
     pick_opacity: bool = False
```

### Comparing `rio_ui-0.7.2/rio/components/component.py` & `rio_ui-0.7.3/rio/components/component.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/components/component_tree.py` & `rio_ui-0.7.3/rio/components/component_tree.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/components/container.py` & `rio_ui-0.7.3/rio/components/container.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/components/devel_component.py` & `rio_ui-0.7.3/rio/components/devel_component.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/components/drawer.py` & `rio_ui-0.7.3/rio/components/drawer.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/components/dropdown.py` & `rio_ui-0.7.3/rio/components/dropdown.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/components/flow_container.py` & `rio_ui-0.7.3/rio/components/flow_container.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/components/fundamental_component.py` & `rio_ui-0.7.3/rio/components/fundamental_component.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/components/grid.py` & `rio_ui-0.7.3/rio/components/grid.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/components/html.py` & `rio_ui-0.7.3/rio/components/html.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/components/icon.py` & `rio_ui-0.7.3/rio/components/icon.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/components/image.py` & `rio_ui-0.7.3/rio/components/image.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/components/key_event_listener.py` & `rio_ui-0.7.3/rio/components/key_event_listener.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/components/labeled_column.py` & `rio_ui-0.7.3/rio/components/labeled_column.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/components/linear_containers.py` & `rio_ui-0.7.3/rio/components/linear_containers.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/components/link.py` & `rio_ui-0.7.3/rio/components/link.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/components/list_items.py` & `rio_ui-0.7.3/rio/components/list_items.py`

 * *Files 2% similar despite different names*

```diff
@@ -266,21 +266,22 @@
     ## Examples
 
     Instead of using the `SimpleListItem` you can use the `CustomListItem` to create
     a custom list item. This can be useful if you want to add more complex content
     to the list item. You can add any component to the list item.
 
     ```python
+    import functools
+
     class MyCustomListItemComponent(rio.Component):
-        # create a custom list item
+        # Create a custom list item
         product: str
         button_text: str
 
         def build(self) -> rio.Component:
-
             return rio.Row(
                 rio.Text(self.product),
                 rio.Spacer(),
                 rio.Button(
                     self.button_text,
                     on_press=lambda: print("Hello, world!"),
                 ),
@@ -296,21 +297,22 @@
         def build(self) -> rio.Component:
             # Store all children in an intermediate list
             list_items = []
 
             for product in self.products:
                 list_items.append(
                     rio.CustomListItem(
-                        # Use the `MyCustomListItem` component to create a custom list item
+                        # Use the `MyCustomListItem` component to create a
+                        # custom list item
                         content=MyCustomListItemComponent(
                             product=product, button_text="Click Me!"
                         ),
                         key=product,
-                        # Note the use of `functools.partial` to pass the product
-                        # to the event handler.
+                        # Note the use of `functools.partial` to pass the
+                        # product to the event handler.
                         on_press=functools.partial(
                             self.on_press_heading_list_item,
                             product=product,
                         ),
                     )
                 )
```

### Comparing `rio_ui-0.7.2/rio/components/list_view.py` & `rio_ui-0.7.3/rio/components/list_view.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/components/markdown.py` & `rio_ui-0.7.3/rio/components/markdown.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/components/media_player.py` & `rio_ui-0.7.3/rio/components/media_player.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/components/mouse_event_listener.py` & `rio_ui-0.7.3/rio/components/mouse_event_listener.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/components/multi_line_text_input.py` & `rio_ui-0.7.3/rio/components/multi_line_text_input.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/components/node_input.py` & `rio_ui-0.7.3/rio/components/node_input.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/components/node_output.py` & `rio_ui-0.7.3/rio/components/node_output.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/components/number_input.py` & `rio_ui-0.7.3/rio/components/number_input.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/components/overlay.py` & `rio_ui-0.7.3/rio/components/overlay.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/components/page_view.py` & `rio_ui-0.7.3/rio/components/page_view.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/components/plot.py` & `rio_ui-0.7.3/rio/components/plot.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/components/popup.py` & `rio_ui-0.7.3/rio/components/popup.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/components/progress_bar.py` & `rio_ui-0.7.3/rio/components/progress_bar.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/components/progress_circle.py` & `rio_ui-0.7.3/rio/components/progress_circle.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/components/rectangle.py` & `rio_ui-0.7.3/rio/components/rectangle.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/components/revealer.py` & `rio_ui-0.7.3/rio/components/revealer.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/components/root_components.py` & `rio_ui-0.7.3/rio/components/root_components.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/components/scroll_container.py` & `rio_ui-0.7.3/rio/components/scroll_container.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/components/scroll_target.py` & `rio_ui-0.7.3/rio/components/scroll_target.py`

 * *Files 13% similar despite different names*

```diff
@@ -35,21 +35,21 @@
     ## Examples
 
     A minimal example of `ScrollTarget` displaying a heading:
 
     ```python
     rio.ScrollTarget(
         id="chapter-1",
-        content=rio.Text('Chapter 1', style='heading1'),
+        content=rio.Text("Chapter 1", style="heading1"),
     )
     ```
 
     ## Metadata
 
-    experimental: True
+    `experimental`: True
     """
 
     id: str
     content: rio.Component | None = None
     _: KW_ONLY
     copy_button_content: str | rio.Component | None = "¶"
     copy_button_spacing: float = 0.5
```

### Comparing `rio_ui-0.7.2/rio/components/separator.py` & `rio_ui-0.7.3/rio/components/separator.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/components/slider.py` & `rio_ui-0.7.3/rio/components/slider.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/components/slideshow.py` & `rio_ui-0.7.3/rio/components/slideshow.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/components/spacer.py` & `rio_ui-0.7.3/rio/components/spacer.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/components/stack.py` & `rio_ui-0.7.3/rio/components/stack.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/components/switch.py` & `rio_ui-0.7.3/rio/components/switch.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/components/switcher.py` & `rio_ui-0.7.3/rio/components/switcher.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/components/switcher_bar.py` & `rio_ui-0.7.3/rio/components/switcher_bar.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/components/table.py` & `rio_ui-0.7.3/rio/components/table.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/components/text.py` & `rio_ui-0.7.3/rio/components/text.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/components/text_input.py` & `rio_ui-0.7.3/rio/components/text_input.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/components/theme_context_switcher.py` & `rio_ui-0.7.3/rio/components/theme_context_switcher.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,29 +21,30 @@
     A `ThemeContextSwitcher` is a container which can switch between different
     components. It is commonly used to switch between different themes. The
     `content` attribute can be used to change the currently displayed component.
 
     You can find more details on theming on the [theming how-to
     page](https://rio.dev/docs/howto/theming).
 
+
     ## Attributes
 
     `content`: The currently displayed component.
 
     `color`: The color of the switcher bar.
 
 
     ## Examples
 
-    A minimal example of a `ThemeContextSwitcher` will be shown:
+    A minimal example of a `ThemeContextSwitcher`:
 
     ```python
     rio.ThemeContextSwitcher(
         content=rio.Button("Button"),
-        color="secondary"
+        color="secondary",
     )
     ```
     """
 
     content: rio.Component
     color: rio.ColorSet
```

### Comparing `rio_ui-0.7.2/rio/components/tooltip.py` & `rio_ui-0.7.3/rio/components/tooltip.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/components/website.py` & `rio_ui-0.7.3/rio/components/website.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/debug/monkeypatches.py` & `rio_ui-0.7.3/rio/debug/monkeypatches.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/debug/typing_utils.py` & `rio_ui-0.7.3/rio/debug/typing_utils.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/debug/validator.py` & `rio_ui-0.7.3/rio/debug/validator.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/debug/dev_tools/component_details.py` & `rio_ui-0.7.3/rio/debug/dev_tools/component_details.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/debug/dev_tools/deploy_page.py` & `rio_ui-0.7.3/rio/debug/dev_tools/deploy_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/debug/dev_tools/dev_tools_sidebar.py` & `rio_ui-0.7.3/rio/debug/dev_tools/dev_tools_sidebar.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/debug/dev_tools/docs_page.py` & `rio_ui-0.7.3/rio/debug/dev_tools/docs_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/debug/dev_tools/icons_page.py` & `rio_ui-0.7.3/rio/debug/dev_tools/icons_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/debug/dev_tools/layout_preview.py` & `rio_ui-0.7.3/rio/debug/dev_tools/layout_preview.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/debug/dev_tools/project_page.py` & `rio_ui-0.7.3/rio/debug/dev_tools/project_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/debug/dev_tools/sample_icons_grid.py` & `rio_ui-0.7.3/rio/debug/dev_tools/sample_icons_grid.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/debug/dev_tools/theme_picker_page.py` & `rio_ui-0.7.3/rio/debug/dev_tools/theme_picker_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/debug/dev_tools/tree_page.py` & `rio_ui-0.7.3/rio/debug/dev_tools/tree_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/docs/__init__.py` & `rio_ui-0.7.3/rio/docs/__init__.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/generated/index.html` & `rio_ui-0.7.3/rio/generated/index.html`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/patches_for_3rd_party_stuff/IocpProactor_accept_locals_accept_coro.py` & `rio_ui-0.7.3/rio/patches_for_3rd_party_stuff/IocpProactor_accept_locals_accept_coro.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/patches_for_3rd_party_stuff/ProactorBasePipeTransport_call_connection_lost.py` & `rio_ui-0.7.3/rio/patches_for_3rd_party_stuff/ProactorBasePipeTransport_call_connection_lost.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/patches_for_3rd_party_stuff/_OverlappedFuture_cancel_overlapped.py` & `rio_ui-0.7.3/rio/patches_for_3rd_party_stuff/_OverlappedFuture_cancel_overlapped.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/snippets/README.md` & `rio_ui-0.7.3/rio/snippets/README.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/snippets/__init__.py` & `rio_ui-0.7.3/rio/snippets/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     "Empty",
     # Sort the remainder alphabetically
     "AI Chatbot",
     "Crypto Dashboard",
     "Multipage Website",
     "Simple CRUD",
     "Tic-Tac-Toe",
+    "Todo App",
 ]
 
 
 @dataclass
 class _TemplateConfig(uniserde.Serde):
     """
     Model for parsing the JSON file which comes along with each project
```

### Comparing `rio_ui-0.7.2/rio/snippets/snippet-files/howtos/core-classes.md` & `rio_ui-0.7.3/rio/snippets/snippet-files/howtos/core-classes.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/snippets/snippet-files/howtos/debugging-setup.md` & `rio_ui-0.7.3/rio/snippets/snippet-files/howtos/debugging-setup.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/snippets/snippet-files/howtos/deployment.md` & `rio_ui-0.7.3/rio/snippets/snippet-files/howtos/deployment.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/snippets/snippet-files/howtos/howto-custom-events.md` & `rio_ui-0.7.3/rio/snippets/snippet-files/howtos/howto-custom-events.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/snippets/snippet-files/howtos/howto-get-value-from-child-component.md` & `rio_ui-0.7.3/rio/snippets/snippet-files/howtos/howto-get-value-from-child-component.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/snippets/snippet-files/howtos/howto-install.md` & `rio_ui-0.7.3/rio/snippets/snippet-files/howtos/howto-install.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/snippets/snippet-files/howtos/howto-pass-value-to-event.md` & `rio_ui-0.7.3/rio/snippets/snippet-files/howtos/howto-pass-value-to-event.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/snippets/snippet-files/howtos/persistent-settings.md` & `rio_ui-0.7.3/rio/snippets/snippet-files/howtos/persistent-settings.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/snippets/snippet-files/howtos/project-setup.md` & `rio_ui-0.7.3/rio/snippets/snippet-files/howtos/project-setup.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/snippets/snippet-files/howtos/run-project.md` & `rio_ui-0.7.3/rio/snippets/snippet-files/howtos/run-project.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/snippets/snippet-files/howtos/theming.md` & `rio_ui-0.7.3/rio/snippets/snippet-files/howtos/theming.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/snippets/snippet-files/other-examples/simple_counter_app.py` & `rio_ui-0.7.3/rio/snippets/snippet-files/other-examples/simple_counter_app.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-AI Chatbot/conversation.py` & `rio_ui-0.7.3/rio/snippets/snippet-files/project-template-AI Chatbot/conversation.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,20 +25,20 @@
     """
 
     # The entire message history
     messages: List[ChatMessage] = field(default_factory=list)
 
     async def respond(self, client: openai.AsyncOpenAI) -> ChatMessage:
         """
-          Creates an AI generated response for this conversation and appends it
-          to the messages list. Also returns the new message.
+        Creates an AI generated response for this conversation and appends it
+        to the messages list. Also returns the new message.
 
         ## Raises
 
-          `ValueError` if the most recent message is not by the user.
+        `ValueError` if the most recent message is not by the user.
         """
 
         # Make sure the last message was by the user
         if not self.messages or self.messages[-1].role != "user":
             raise ValueError("The most recent message must be by the user")
 
         # Convert all messages to the format needed by the API
```

### Comparing `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-AI Chatbot/root_init.py` & `rio_ui-0.7.3/rio/snippets/snippet-files/project-template-AI Chatbot/root_init.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-AI Chatbot/thumbnail.svg` & `rio_ui-0.7.3/rio/snippets/snippet-files/project-template-AI Chatbot/thumbnail.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_message.py` & `rio_ui-0.7.3/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_message.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_suggestion_card.py` & `rio_ui-0.7.3/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_suggestion_card.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-AI Chatbot/components/empty_chat_placeholder.py` & `rio_ui-0.7.3/rio/snippets/snippet-files/project-template-AI Chatbot/components/empty_chat_placeholder.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-AI Chatbot/components/generating_response_placeholder.py` & `rio_ui-0.7.3/rio/snippets/snippet-files/project-template-AI Chatbot/components/generating_response_placeholder.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-AI Chatbot/pages/chat_page.py` & `rio_ui-0.7.3/rio/snippets/snippet-files/project-template-AI Chatbot/pages/chat_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Crypto Dashboard/data_models.py` & `rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Crypto Dashboard/data_models.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Crypto Dashboard/thumbnail.svg` & `rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Crypto Dashboard/thumbnail.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Crypto Dashboard/assets/cryptos.csv` & `rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Crypto Dashboard/assets/cryptos.csv`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/balance_card.py` & `rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/balance_card.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_card.py` & `rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_card.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_chart.py` & `rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_chart.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Crypto Dashboard/pages/dashboard_page.py` & `rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Crypto Dashboard/pages/dashboard_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Empty/thumbnail.svg` & `rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Empty/thumbnail.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Empty/pages/sample_page.py` & `rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Empty/pages/sample_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Multipage Website/README.md` & `rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Multipage Website/README.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Multipage Website/thumbnail.svg` & `rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Multipage Website/thumbnail.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Multipage Website/components/footer.py` & `rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Multipage Website/components/footer.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Multipage Website/components/navbar.py` & `rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Multipage Website/components/navbar.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Multipage Website/components/testimonial.py` & `rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Multipage Website/components/testimonial.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Multipage Website/pages/about_page.py` & `rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Multipage Website/pages/about_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Multipage Website/pages/home_page.py` & `rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Multipage Website/pages/home_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Multipage Website/pages/news_page.py` & `rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Multipage Website/pages/news_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Multipage Website/pages/root_page.py` & `rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Multipage Website/pages/root_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Simple CRUD/data_models.py` & `rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Simple CRUD/data_models.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Simple CRUD/thumbnail.svg` & `rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Simple CRUD/thumbnail.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_editor.py` & `rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_editor.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_list.py` & `rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_list.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Simple CRUD/pages/crud_page.py` & `rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Simple CRUD/pages/crud_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/thumbnail.svg` & `rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/thumbnail.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/field.py` & `rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/field.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/tic_tac_toe_page.py` & `rio_ui-0.7.3/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/tic_tac_toe_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/tic_tac_toe_page.py` & `rio_ui-0.7.3/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/tic_tac_toe_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/field.py` & `rio_ui-0.7.3/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/field.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/tic_tac_toe_page.py` & `rio_ui-0.7.3/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/tic_tac_toe_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/field.py` & `rio_ui-0.7.3/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/field.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/tic_tac_toe_page.py` & `rio_ui-0.7.3/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/tic_tac_toe_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/field.py` & `rio_ui-0.7.3/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/field.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/tic_tac_toe_page.py` & `rio_ui-0.7.3/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/tic_tac_toe_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/scripts/benchmark.py` & `rio_ui-0.7.3/scripts/benchmark.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/scripts/build_material_icon_set.py` & `rio_ui-0.7.3/scripts/build_material_icon_set.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/scripts/code_coverage.py` & `rio_ui-0.7.3/scripts/code_coverage.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/scripts/publish_new_release.py` & `rio_ui-0.7.3/scripts/publish_new_release.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/tests/test_custom_components.py` & `rio_ui-0.7.3/tests/test_custom_components.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import dataclasses
 
-from utils import create_mockapp, enable_component_instantiation
+from utils import enable_component_instantiation
 
-import rio
+import rio.testing
 
 
 @enable_component_instantiation
 def test_fields_with_defaults():
     class TestComponent(rio.Component):
         foo: list[str] = dataclasses.field(init=False, default_factory=list)
         bar: int = dataclasses.field(init=False, default=5)
@@ -25,10 +25,10 @@
 
         def __post_init__(self):
             self.post_init_called = True
 
         def build(self) -> rio.Component:
             return rio.Text("hi")
 
-    async with create_mockapp(TestComponent) as app:
-        root_component = app.get_component(TestComponent)
+    async with rio.testing.TestClient(TestComponent) as test_client:
+        root_component = test_client.get_component(TestComponent)
         assert root_component.post_init_called
```

### Comparing `rio_ui-0.7.2/tests/test_docstring_code_blocks.py` & `rio_ui-0.7.3/tests/test_docstring_code_blocks.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,115 +1,127 @@
 import re
 import subprocess
+import sys
 import tempfile
+import textwrap
 from typing import *  # type: ignore
 
 import black
-import imy.docstrings
 import pyright
 import pytest
 
-import rio
+import rio.docs
 
-CODE_BLOCK_PATTERN = re.compile(r"```.*?\n(.*?)\n```", re.DOTALL)
+CODE_BLOCK_PATTERN = re.compile(r"```(.*?)```", re.DOTALL)
 
 
-def all_components() -> list[Type[rio.Component]]:
-    """
-    Iterates over all components that ship with Rio.
-    """
-    to_do: Iterable[Type[rio.Component]] = [rio.Component]
-    result: list[Type[rio.Component]] = []
-
-    while to_do:
-        component = to_do.pop()
-        result.append(component)
-        to_do.extend(component.__subclasses__())
-
-    return result
+all_documented_objects = [
+    obj for obj, _ in rio.docs.find_documented_objects(False)
+]
+all_documented_objects.sort(key=lambda obj: obj.__name__)
 
 
-def get_code_blocks(comp: Type[rio.Component]) -> list[str]:
+def get_code_blocks(obj: type | Callable) -> list[str]:
     """
     Returns a list of all code blocks in the docstring of a component.
     """
-    docs = imy.docstrings.ClassDocs.from_class(comp)
+    docstring = obj.__doc__
 
     # No docs?
-    if docs.details is None:
+    if not docstring:
         return []
 
+    docstring = textwrap.dedent(docstring)
+
     # Find any contained code blocks
     result: list[str] = []
-    for match in CODE_BLOCK_PATTERN.finditer(docs.details):
-        block: str = match.group(0)
-
-        assert block.startswith("```")
-        assert block.endswith("```")
+    for match in CODE_BLOCK_PATTERN.finditer(docstring):
+        block: str = match.group(1)
 
         # Split into language and source
-        linebreak = block.index("\n")
+        linebreak = block.find("\n")
         assert linebreak != -1
-        first_line = block[3:linebreak].strip()
-        block = block[linebreak + 1 : -3]
+        language = block[:linebreak]
+        block = block[linebreak + 1 :]
 
         # Make sure a language is specified
-        assert first_line, "The code block has no language specified"
+        assert language, "The code block has no language specified"
 
         result.append(block)
 
     return result
 
 
-@pytest.mark.parametrize("comp", all_components())
-def test_eval_code_block(comp: Type[rio.Component]) -> None:
+@pytest.mark.parametrize("obj", all_documented_objects)
+def test_eval_code_block(obj: type | Callable) -> None:
     # Eval all code blocks and make sure they don't crash
-    for source in get_code_blocks(comp):
+    for source in get_code_blocks(obj):
         compile(source, "<string>", "exec")
 
 
-@pytest.mark.parametrize("comp", all_components())
-def test_code_block_is_formatted(comp: Type[rio.Component]) -> None:
+@pytest.mark.parametrize("obj", all_documented_objects)
+def test_code_block_is_formatted(obj: type | Callable) -> None:
     # Make sure all code blocks are formatted according to black
-    for source in get_code_blocks(comp):
+    for source in get_code_blocks(obj):
         formatted_source = black.format_str(source, mode=black.FileMode())
+
+        # Black often inserts 2 empty lines between stuff, but that's really not
+        # necessary in docstrings. So we'll collapse those into a single empty
+        # line.
+        source = source.replace("\n\n\n", "\n\n")
+        formatted_source = formatted_source.replace("\n\n\n", "\n\n")
+
         assert source == formatted_source
 
 
-def _pyright_check_source(source: str) -> tuple[int, int]:
+PYRIGHT_ERROR_OR_WARNING_REGEX = re.compile(
+    r".*\.py:\d+:\d+ - (?:error|warning): (.*)"
+)
+
+
+def _find_static_typing_errors(source: str) -> str:
     """
     Run pyright on the given source and return the number of errors and
     warnings.
     """
     with tempfile.NamedTemporaryFile(suffix=".py") as f:
         # Dump the source to a file, and implicitly import rio
         f.write("import rio\n".encode("utf-8"))
         f.write(source.encode("utf-8"))
         f.flush()
 
         # Run pyright
         proc = pyright.run(
+            "--pythonpath",
+            sys.executable,
             f.name,
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
         )
         result_out = proc.stdout
         assert isinstance(result_out, bytes), type(result_out)
         result_out = result_out.decode()
 
         # Find the number of errors and warnings
-        match = re.search(
-            r"(\d+) error(s)?, (\d+) warning(s)?, (\d+) information",
-            result_out,
-        )
-        assert match is not None, result_out
-        return int(match.group(1)), int(match.group(3))
+        lines = list[str]()
 
+        for line in result_out.splitlines():
+            match = PYRIGHT_ERROR_OR_WARNING_REGEX.match(line)
 
-@pytest.mark.parametrize("comp", all_components())
-def test_analyze_code_block(comp: Type[rio.Component]) -> None:
-    # Make sure pyright is happy with all code blocks
-    for source in get_code_blocks(comp):
-        n_errors, n_warnings = _pyright_check_source(source)
+            if match:
+                lines.append(match.group(1))
 
-        assert n_errors == 0, f"Found {n_errors} errors"
-        assert n_warnings == 0, f"Found {n_warnings} warnings"
+        return "\n".join(lines)
+
+
+@pytest.mark.parametrize("obj", all_documented_objects)
+def test_analyze_code_block(obj: type | Callable) -> None:
+    # A lot of snippets are missing context, so it's only natural that pyright
+    # will find issues with the code. There isn't really anything we can do
+    # about it, so we'll just skip those object.
+    if obj in (rio.App, rio.Color, rio.UserSettings):
+        pytest.xfail()
+
+    # Make sure pyright is happy with all code blocks
+    for source in get_code_blocks(obj):
+        errors = _find_static_typing_errors(source)
+        assert not errors, errors
```

### Comparing `rio_ui-0.7.2/tests/test_documentation.py` & `rio_ui-0.7.3/tests/test_documentation.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/tests/test_events.py` & `rio_ui-0.7.3/tests/test_events.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import asyncio
 
-from utils import create_mockapp
-
-import rio
+import rio.testing
 
 
 class ChildToggler(rio.Component):
     child: rio.Component
     switch: bool = True
 
     def toggle(self) -> None:
@@ -35,45 +33,45 @@
 
         def build(self) -> rio.Component:
             return rio.Text("hi")
 
     def build():
         return ChildToggler(DemoComponent())
 
-    async with create_mockapp(build) as app:
-        root = app.get_component(ChildToggler)
+    async with rio.testing.TestClient(build) as test_client:
+        root = test_client.get_component(ChildToggler)
         assert not mounted
         assert not unmounted
 
         root.toggle()
-        await app.refresh()
+        await test_client.refresh()
         assert mounted
         assert not unmounted
 
         root.toggle()
-        await app.refresh()
+        await test_client.refresh()
         assert unmounted
 
 
 async def test_refresh_after_synchronous_mount_handler():
     class DemoComponent(rio.Component):
         mounted: bool = False
 
         @rio.event.on_mount
         def on_mount(self):
             self.mounted = True
 
         def build(self) -> rio.Component:
             return rio.Switch(self.mounted)
 
-    async with create_mockapp(DemoComponent) as app:
-        demo_component = app.get_component(DemoComponent)
-        switch = app.get_component(rio.Switch)
+    async with rio.testing.TestClient(DemoComponent) as test_client:
+        demo_component = test_client.get_component(DemoComponent)
+        switch = test_client.get_component(rio.Switch)
 
         # TODO: I don't know how we can wait for the refresh, so I'll just use a
         # sleep()
         await asyncio.sleep(0.5)
         assert demo_component.mounted
 
-        last_component_state_changes = app.last_component_state_changes
+        last_component_state_changes = test_client._last_component_state_changes
         assert switch in last_component_state_changes
         assert last_component_state_changes[switch].get("is_on") is True
```

### Comparing `rio_ui-0.7.2/tests/test_project_templates.py` & `rio_ui-0.7.3/tests/test_project_templates.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/tests/test_reconciliation.py` & `rio_ui-0.7.3/tests/test_reconciliation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-from utils import create_mockapp
-
-import rio
+import rio.testing
 
 
 async def test_default_values_arent_considered_explicitly_set():
     class SquareComponent(rio.Component):
         label: str
 
         def __init__(self, label: str, size: float = 5):
@@ -18,17 +16,19 @@
     class RootComponent(rio.Component):
         text: str
 
         def build(self):
             square_component = SquareComponent(self.text, size=10)
             return rio.Container(square_component)
 
-    async with create_mockapp(lambda: RootComponent("Hello")) as app:
-        root_component = app.get_component(RootComponent)
-        square_component = app.get_component(SquareComponent)
+    async with rio.testing.TestClient(
+        lambda: RootComponent("Hello")
+    ) as test_client:
+        root_component = test_client.get_component(RootComponent)
+        square_component = test_client.get_component(SquareComponent)
 
         # Create a new SquareComponent with the default size. Since we aren't
         # explicitly passing a size to the constructor, reconciliation should
         # keep the old size.
         root_component.text = "World"
         await root_component.force_refresh()
 
@@ -37,28 +37,29 @@
         assert square_component.height == 10
 
 
 async def test_reconcile_same_component_instance():
     def build():
         return rio.Container(rio.Text("Hello"))
 
-    async with create_mockapp(build) as app:
-        app.outgoing_messages.clear()
+    async with rio.testing.TestClient(build) as test_client:
+        test_client._outgoing_messages.clear()
 
-        root_component = app.get_component(rio.Container)
+        root_component = test_client.get_component(rio.Container)
         await root_component.force_refresh()
 
         # Nothing changed, so there's no need to send any data to JS. But in
         # order to know that nothing changed, the framework would have to track
         # every individual attribute of every component. Since we forced the
-        # root_component to refresh, it's reasonable to send that component's data to
-        # JS.
-        assert not app.outgoing_messages or app.last_updated_components == {
-            root_component
-        }
+        # root_component to refresh, it's reasonable to send that component's
+        # data to JS.
+        assert (
+            not test_client._outgoing_messages
+            or test_client._last_updated_components == {root_component}
+        )
 
 
 async def test_reconcile_not_dirty_high_level_component():
     # Situation:
     # HighLevelComponent1 contains HighLevelComponent2
     # HighLevelComponent2 contains LowLevelContainer
     # HighLevelComponent1 is rebuilt and changes the child of LowLevelContainer
@@ -81,22 +82,22 @@
 
     class HighLevelComponent2(rio.Component):
         content: rio.Component
 
         def build(self):
             return self.content
 
-    async with create_mockapp(HighLevelComponent1) as app:
-        root_component = app.get_component(HighLevelComponent1)
+    async with rio.testing.TestClient(HighLevelComponent1) as test_client:
+        root_component = test_client.get_component(HighLevelComponent1)
         root_component.switch = True
-        await app.refresh()
+        await test_client.refresh()
 
         assert any(
             isinstance(component, rio.Switch)
-            for component in app.last_updated_components
+            for component in test_client._last_updated_components
         )
 
 
 async def test_reconcile_unusual_types():
     class Container(rio.Component):
         def build(self) -> rio.Component:
             return CustomComponent(
@@ -111,16 +112,16 @@
         text: str
         tuple: tuple[float, rio.Component]
         byte_array: bytearray
 
         def build(self):
             return rio.Text(self.text)
 
-    async with create_mockapp(Container) as app:
-        root_component = app.get_component(Container)
+    async with rio.testing.TestClient(Container) as test_client:
+        root_component = test_client.get_component(Container)
 
         # As long as this doesn't crash, it's fine
         await root_component.force_refresh()
 
 
 async def test_reconcile_by_key():
     class Toggler(rio.Component):
@@ -128,57 +129,57 @@
 
         def build(self):
             if not self.toggle:
                 return rio.Text("Hello", key="foo")
             else:
                 return rio.Container(rio.Text("World", key="foo"))
 
-    async with create_mockapp(Toggler) as app:
-        root_component = app.get_component(Toggler)
-        text = app.get_component(rio.Text)
+    async with rio.testing.TestClient(Toggler) as test_client:
+        root_component = test_client.get_component(Toggler)
+        text = test_client.get_component(rio.Text)
 
         root_component.toggle = True
-        await app.refresh()
+        await test_client.refresh()
 
         assert text.text == "World"
 
 
 async def test_key_prevents_structural_match():
     class Toggler(rio.Component):
         toggle: bool = False
 
         def build(self):
             if not self.toggle:
                 return rio.Text("Hello")
             else:
                 return rio.Text("World", key="foo")
 
-    async with create_mockapp(Toggler) as app:
-        root_component = app.get_component(Toggler)
-        text = app.get_component(rio.Text)
+    async with rio.testing.TestClient(Toggler) as test_client:
+        root_component = test_client.get_component(Toggler)
+        text = test_client.get_component(rio.Text)
 
         root_component.toggle = True
-        await app.refresh()
+        await test_client.refresh()
 
         assert text.text == "Hello"
 
 
 async def test_key_interrupts_structure():
     class Toggler(rio.Component):
         key_: str = "abc"
 
         def build(self):
             return rio.Container(rio.Text(self.key_), key=self.key_)
 
-    async with create_mockapp(Toggler) as app:
-        root_component = app.get_component(Toggler)
-        text = app.get_component(rio.Text)
+    async with rio.testing.TestClient(Toggler) as test_client:
+        root_component = test_client.get_component(Toggler)
+        text = test_client.get_component(rio.Text)
 
         root_component.key_ = "123"
-        await app.refresh()
+        await test_client.refresh()
 
         # The container's key changed, so even though the structure is the same,
         # the old Text component should be unchanged.
         assert text.text == "abc"
 
 
 async def test_structural_matching_inside_keyed_component():
@@ -190,20 +191,20 @@
                 return rio.Row(rio.Container(rio.Text("A"), key="foo"))
             else:
                 return rio.Row(
                     rio.Container(rio.Text("B")),
                     rio.Container(rio.Text("C"), key="foo"),
                 )
 
-    async with create_mockapp(Toggler) as app:
-        root_component = app.get_component(Toggler)
-        text = app.get_component(rio.Text)
+    async with rio.testing.TestClient(Toggler) as test_client:
+        root_component = test_client.get_component(Toggler)
+        text = test_client.get_component(rio.Text)
 
         root_component.toggle = True
-        await app.refresh()
+        await test_client.refresh()
 
         # The container with key "foo" has moved. Make sure the structure inside
         # of it was reconciled correctly.
         assert text.text == "C"
 
 
 async def test_key_matching_inside_keyed_component():
@@ -221,20 +222,20 @@
             else:
                 return rio.Row(
                     rio.Text("B"),
                     rio.Container(rio.Text("C"), key="container"),
                     key="row",
                 )
 
-    async with create_mockapp(Toggler) as app:
-        root_component = app.get_component(Toggler)
-        text = app.get_component(rio.Text)
+    async with rio.testing.TestClient(Toggler) as test_client:
+        root_component = test_client.get_component(Toggler)
+        text = test_client.get_component(rio.Text)
 
         root_component.toggle = True
-        await app.refresh()
+        await test_client.refresh()
 
         # The container with key "foo" has moved. Make sure the structure inside
         # of it was reconciled correctly.
         assert text.text == "C"
 
 
 async def test_same_key_on_different_component_type():
@@ -249,57 +250,57 @@
 
         def build(self):
             if not self.toggle:
                 return rio.Text("Hello", key="foo")
             else:
                 return ComponentWithText("World", key="foo")
 
-    async with create_mockapp(Toggler) as app:
-        root_component = app.get_component(Toggler)
-        text = app.get_component(rio.Text)
+    async with rio.testing.TestClient(Toggler) as test_client:
+        root_component = test_client.get_component(Toggler)
+        text = test_client.get_component(rio.Text)
 
         root_component.toggle = True
-        await app.refresh()
+        await test_client.refresh()
 
         assert text.text == "Hello"
 
 
 async def test_text_reconciliation():
     class RootComponent(rio.Component):
         text: str = "foo"
 
         def build(self) -> rio.Component:
             return rio.Text(self.text)
 
-    async with create_mockapp(RootComponent) as app:
-        root = app.get_component(RootComponent)
-        text = app.get_component(rio.Text)
+    async with rio.testing.TestClient(RootComponent) as test_client:
+        root = test_client.get_component(RootComponent)
+        text = test_client.get_component(rio.Text)
 
         root.text = "bar"
-        await app.refresh()
+        await test_client.refresh()
 
         assert text.text == root.text
 
 
 async def test_grid_reconciliation():
     class RootComponent(rio.Component):
         num_rows: int = 1
 
         def build(self) -> rio.Component:
             rows = [[rio.Text(f"Row {n}")] for n in range(self.num_rows)]
             return rio.Grid(*rows)
 
-    async with create_mockapp(RootComponent) as app:
-        root = app.get_component(RootComponent)
-        grid = app.get_component(rio.Grid)
+    async with rio.testing.TestClient(RootComponent) as test_client:
+        root = test_client.get_component(RootComponent)
+        grid = test_client.get_component(rio.Grid)
 
         root.num_rows += 1
-        await app.refresh()
+        await test_client.refresh()
 
-        assert {root, grid} < app.last_updated_components
+        assert {root, grid} < test_client._last_updated_components
         assert len(grid._children) == root.num_rows
 
 
 async def test_margin_reconciliation():
     class RootComponent(rio.Component):
         switch: bool = True
 
@@ -313,20 +314,20 @@
                     rio.Text("hi", margin_top=1),
                     rio.Text("hi", margin_bottom=1),
                     rio.Text("hi", margin_x=1),
                     rio.Text("hi", margin_y=1),
                     rio.Text("hi", margin=1),
                 )
 
-    async with create_mockapp(RootComponent) as app:
-        root = app.get_component(RootComponent)
-        texts = list(app.get_components(rio.Text))
+    async with rio.testing.TestClient(RootComponent) as test_client:
+        root = test_client.get_component(RootComponent)
+        texts = list(test_client.get_components(rio.Text))
 
         root.switch = False
-        await app.refresh()
+        await test_client.refresh()
 
         assert texts[0].margin_left == 1
         assert texts[1].margin_right == 1
         assert texts[2].margin_top == 1
         assert texts[3].margin_bottom == 1
 
         assert texts[4].margin_x == 1
@@ -355,21 +356,27 @@
 
         def build(self) -> rio.Component:
             return self.child
 
     def build() -> rio.Component:
         return Container(rio.Text("foo"))
 
-    async with create_mockapp(build, use_ordered_dirty_set=True) as app:
-        container = app.get_component(Container)
-        child = app.get_component(rio.Text)
+    async with rio.testing.TestClient(
+        build, use_ordered_dirty_set=True
+    ) as test_client:
+        container = test_client.get_component(Container)
+        child = test_client.get_component(rio.Text)
 
         # Change the child's state and make its parent rebuild
         child.text = "bar"
         container.child = child
 
         # In order for the bug to occur, the parent has to be rebuilt before the
         # child
-        assert list(app.session._dirty_components) == [child, container]
-        await app.refresh()
+        assert test_client._session is not None
+        assert list(test_client._session._dirty_components) == [
+            child,
+            container,
+        ]
+        await test_client.refresh()
 
-        assert app.last_updated_components == {child, container}
+        assert test_client._last_updated_components == {child, container}
```

### Comparing `rio_ui-0.7.2/tests/test_refresh.py` & `rio_ui-0.7.3/tests/test_refresh.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,34 @@
-from utils import create_mockapp
-
-import rio
+import rio.testing
 
 
 async def test_refresh_with_nothing_to_do():
     def build():
         return rio.Text("Hello")
 
-    async with create_mockapp(build) as app:
-        app.outgoing_messages.clear()
-        await app.refresh()
+    async with rio.testing.TestClient(build) as test_client:
+        test_client._outgoing_messages.clear()
+        await test_client.refresh()
 
-        assert not app.dirty_components
-        assert not app.last_updated_components
+        assert not test_client._dirty_components
+        assert not test_client._last_updated_components
 
 
 async def test_refresh_with_clean_root_component():
     def build():
         text_component = rio.Text("Hello")
         return rio.Container(text_component)
 
-    async with create_mockapp(build) as app:
-        text_component = app.get_component(rio.Text)
+    async with rio.testing.TestClient(build) as test_client:
+        text_component = test_client.get_component(rio.Text)
 
         text_component.text = "World"
-        await app.refresh()
+        await test_client.refresh()
 
-        assert app.last_updated_components == {text_component}
+        assert test_client._last_updated_components == {text_component}
 
 
 async def test_rebuild_component_with_dead_parent():
     class RootComponent(rio.Component):
         content: rio.Component
 
         def build(self) -> rio.Component:
@@ -46,28 +44,28 @@
         return RootComponent(
             rio.Row(
                 ComponentWithState("Hello"),
                 rio.ProgressCircle(),
             )
         )
 
-    async with create_mockapp(build) as app:
+    async with rio.testing.TestClient(build) as test_client:
         # Change the component's state, but also remove its parent from the
         # component tree
-        root_component = app.get_component(RootComponent)
-        component = app.get_component(ComponentWithState)
-        progress_component = app.get_component(rio.ProgressCircle)
+        root_component = test_client.get_component(RootComponent)
+        component = test_client.get_component(ComponentWithState)
+        progress_component = test_client.get_component(rio.ProgressCircle)
 
         component.state = "Hi"
         root_component.content = progress_component
 
-        await app.refresh()
+        await test_client.refresh()
 
         # Make sure no data for dead components was sent to JS
-        assert app.last_updated_components == {root_component}
+        assert test_client._last_updated_components == {root_component}
 
 
 async def test_unmount_and_remount():
     class DemoComponent(rio.Component):
         content: rio.Component
         show_child: bool
 
@@ -77,23 +75,26 @@
 
     def build() -> rio.Component:
         return DemoComponent(
             rio.Text("hi"),
             show_child=True,
         )
 
-    async with create_mockapp(build) as app:
-        root_component = app.get_component(DemoComponent)
+    async with rio.testing.TestClient(build) as test_client:
+        root_component = test_client.get_component(DemoComponent)
         child_component = root_component.content
-        row_component = app.get_component(rio.Row)
+        row_component = test_client.get_component(rio.Row)
 
         root_component.show_child = False
-        await app.refresh()
-        assert app.last_updated_components == {root_component, row_component}
+        await test_client.refresh()
+        assert test_client._last_updated_components == {
+            root_component,
+            row_component,
+        }
 
         root_component.show_child = True
-        await app.refresh()
-        assert app.last_updated_components == {
+        await test_client.refresh()
+        assert test_client._last_updated_components == {
             root_component,
             row_component,
             child_component,
         }
```

### Comparing `rio_ui-0.7.2/tests/test_session.py` & `rio_ui-0.7.3/tests/test_session.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,45 +1,42 @@
 import pytest
-from utils import create_mockapp
 
-import rio
+import rio.testing
 
 
-async def test_session_attachments():
-    async with create_mockapp() as app:
-        session = app.session
+async def test_client_attachments():
+    async with rio.testing.TestClient() as test_client:
+        session = test_client.session
 
         list1 = ["foo", "bar"]
         list2 = []
 
         session.attach(list1)
         assert session[list] is list1
 
         session.attach(list2)
         assert session[list] is list2
 
 
 async def test_access_nonexistent_session_attachment():
-    async with create_mockapp() as app:
-        session = app.session
-
+    async with rio.testing.TestClient() as test_client:
         with pytest.raises(KeyError):
-            session[list]
+            test_client.session[list]
 
 
 async def test_default_attachments():
     class Settings(rio.UserSettings):
         foo: int
 
     dict_attachment = {"foo": "bar"}
     settings_attachment = Settings(3)
 
-    async with create_mockapp(
+    async with rio.testing.TestClient(
         default_attachments=[dict_attachment, settings_attachment]
-    ) as app:
-        session = app.session
+    ) as test_client:
+        session = test_client.session
 
         # Default attachments shouldn't be copied, unless they're UserSettings
         assert session[dict] is dict_attachment
 
-        assert session[Settings] == settings_attachment
         assert session[Settings] is not settings_attachment
+        assert session[Settings]._equals(settings_attachment)
```

### Comparing `rio_ui-0.7.2/tests/test_zzz_guardrails.py` & `rio_ui-0.7.3/tests/test_zzz_guardrails.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # The "zzz" in the file name is there to ensure that this file runs last, so
 # that the remaining tests run without the monkeypatches applied.
 
 import pytest
-from utils import create_mockapp, enable_component_instantiation
+from utils import enable_component_instantiation
 
-import rio
+import rio.testing
 from rio.debug.monkeypatches import apply_monkeypatches
 
 apply_monkeypatches()
 
 
 def test_components_cant_be_instantiated_outside_of_build_methods():
     with pytest.raises(Exception):
@@ -58,29 +58,14 @@
 @enable_component_instantiation
 def test_component_class_can_be_used_as_build_function(
     component_cls: type[rio.Component],
 ):
     _ = rio.PageView(fallback_build=component_cls)
 
 
-@pytest.mark.parametrize(
-    "component_cls",
-    [
-        rio.Dropdown,
-        rio.Text,
-    ],
-)
-@enable_component_instantiation
-def test_component_class_cant_be_used_as_build_function(
-    component_cls: type[rio.Component],
-):
-    with pytest.raises(Exception):
-        _ = rio.PageView(fallback_build=component_cls)
-
-
 async def test_init_cannot_read_state_properties():
     # Accessing state properties in `__init__` is not allowed because state
     # bindings aren't initialized yet at that point. In development mode, trying
     # to access a state property in `__init__` should raise an exception.
     init_executed = False
     accessing_foo_raised_exception = accessing_margin_top_raised_exception = (
         False
@@ -112,11 +97,11 @@
         def build(self) -> rio.Component:
             return rio.Text("hi", margin_top=self.margin_top)
 
     class Container(rio.Component):
         def build(self) -> rio.Component:
             return IllegalComponent(17)
 
-    async with create_mockapp(Container):
+    async with rio.testing.TestClient(Container):
         assert init_executed
         assert accessing_foo_raised_exception
         assert accessing_margin_top_raised_exception
```

### Comparing `rio_ui-0.7.2/LICENSE.txt` & `rio_ui-0.7.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/README.md` & `rio_ui-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.7.2/pyproject.toml` & `rio_ui-0.7.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -14,26 +14,25 @@
     "httpx~=0.25.1",
     "imy~=0.3.2",
     "introspection~=1.8",
     "isort~=5.13.2",
     "keyring~=24.3.0",
     "matplotlib>=3.8.4",
     "pillow~=10.2.0",
-    "plotly>=5.22.0",
     "pytest~=7.3.1",
     "python-levenshtein~=0.23.0",
     "python-multipart~=0.0.6",
     "pytz~=2024.1",
     "revel~=0.9.1",
     "timer-dict~=1.0.0",
     "tomlkit~=0.12.3",
     "typing-extensions>=4.5.0",
     "unicall~=0.1.5",
     "uniserde~=0.3.13",
-    "uvicorn[standard]~=0.23.2",
+    "uvicorn[standard]~=0.29.0",
     "watchfiles~=0.21.0",
     "yarl>=1.9.4",
 ]
 requires-python = ">= 3.10"
 readme = "README.md"
 license.file = "LICENSE.txt"
 keywords = [
@@ -88,27 +87,27 @@
 build-backend = "hatchling.build"
 
 [tool.rye]
 dev-dependencies = [
     "alt-pytest-asyncio~=0.7.2",
     "black~=24.4.0",
     "coverage~=7.2.2",
+    "plotly>=5.22.0",
     "pre-commit~=3.1.1",
     "pytest~=7.3.1",
     "pyright~=1.1.350",
     "requests~=2.31",
     "ruff~=0.4.1",
     "pandas>=2.2.2",
     "polars>=0.20.23",
     "pywebview",
 ]
 managed = true
 
 [tool.rye.scripts]
-# check-docs = { call = "scripts.check_docs:main" }
 build = "npm run build"
 dev-build = "npm run dev-build"
 publish = { call = "scripts.publish_new_release:main" }
 
 [tool.hatch.version]
 path = "rio/__init__.py"
```

### Comparing `rio_ui-0.7.2/PKG-INFO` & `rio_ui-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: rio-ui
-Version: 0.7.2
+Version: 0.7.3
 Summary: Build modern Websites and Apps just with Python
 Project-URL: homepage, https://rio.dev
 Project-URL: documentation, https://rio.dev/docs
 Author-email: Jakob Pinterits <jakob.pinterits@gmail.com>, Paul Pinterits <rawing7@gmail.com>
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -228,26 +228,25 @@
 Requires-Dist: httpx~=0.25.1
 Requires-Dist: imy~=0.3.2
 Requires-Dist: introspection~=1.8
 Requires-Dist: isort~=5.13.2
 Requires-Dist: keyring~=24.3.0
 Requires-Dist: matplotlib>=3.8.4
 Requires-Dist: pillow~=10.2.0
-Requires-Dist: plotly>=5.22.0
 Requires-Dist: pytest~=7.3.1
 Requires-Dist: python-levenshtein~=0.23.0
 Requires-Dist: python-multipart~=0.0.6
 Requires-Dist: pytz~=2024.1
 Requires-Dist: revel~=0.9.1
 Requires-Dist: timer-dict~=1.0.0
 Requires-Dist: tomlkit~=0.12.3
 Requires-Dist: typing-extensions>=4.5.0
 Requires-Dist: unicall~=0.1.5
 Requires-Dist: uniserde~=0.3.13
-Requires-Dist: uvicorn[standard]~=0.23.2
+Requires-Dist: uvicorn[standard]~=0.29.0
 Requires-Dist: watchfiles~=0.21.0
 Requires-Dist: yarl>=1.9.4
 Provides-Extra: window
 Requires-Dist: cefpython3~=66.1; (sys_platform == 'win32') and extra == 'window'
 Requires-Dist: platformdirs~=3.11.0; extra == 'window'
 Requires-Dist: pygobject~=3.44.1; (sys_platform == 'linux') and extra == 'window'
 Requires-Dist: pywebview~=4.2.2; extra == 'window'
```

