<template>
    <Layout>
        <section data-bs-version="5.1" class="content6 cid-txwAxKl8iA" id="content6-v">

            <div class="container">
                <div class="row justify-content-center">
                    <div class="col-md-12 col-lg-10">
                        <hr class="line">
                        <p class="mbr-text align-center mbr-fonts-style my-4 display-7"><strong>Roadmap and Change Log
                                <br></strong>
                            <br>paint.net 5.0.2 - released on February 19th, 2023
                            <br>This is a small update with some performance improvements, bug fixes, and updates to the
                            bundled plugins.
                            <br>
                            <br>New Adjustment: Invert Alpha
                            <br>Greatly improved performance for some distortion effects (Bulge, Crystalize, Dents,
                            Frosted Glass)
                            <br>Improved performance with large images, especially when making small/quick edits
                            <br>Fixed keyboard tabbing between the Width and Height text boxes in the toolbar when using
                            Fixed Ratio or Fixed Size with the Rectangle Select tool
                            <br>Fixed Bokeh blur effect's handling of the alpha channel for images with transparency
                            <br>Fixed the keyboard up/down increments for the Offset property in the Drop Shadow effect
                            <br>Fixed compatibility with the Lightning effect plugin
                            <br>Fixed compatibility with the ApplyTexture effect plugin
                            <br>Removed keyboard shortcuts for Image -&gt; Rotate 90° Counter-clockwise and Rotate 180°
                            <br>Updated the bundled AvifFileType plugin to version 1.1.24.0 (thanks @null54!)
                            <br>Updated the bundled DDSFileTypePlus plugin to version 1.11.1.0 (thanks @null54!)
                            <br>
                            <br>
                            <br>paint.net 5.0.1 - released on January 21st, 2023
                            <br>This is a small update with a few important bug fixes, updates to the bundled plugins,
                            and a new toolbar button to enable/disable pressure sensitivity.
                            <br>New: Added a button in the toolbar, next to Brush Size, for enabling/disabling pressure
                            sensitivity. The button will only appear if a compatible pen or drawing tablet is detected,
                            and Windows Ink has not been disabled in Settings.
                            <br>Fixed some issues with the main window that would only happen on multimonitor Windows 10
                            systems
                            <br>Fixed a few small issues with the Zoom tool
                            <br>Fixed an issue when saving a JPEG or TIFF with certain types of 0-length IPTC metadata
                            <br>Fixed: On older systems with multiple GPUs (e.g. Intel HD iGPU and an AMD/NVIDIA dGPU),
                            where the first enumerated GPU does not support Direct3D 11, PDN will now use the next
                            enumerated GPU that meets the Direct3D 11 requirement, rather than falling back to CPU
                            rendering.
                            <br>Fixed a rendering bug when using the Pencil tool on small images exactly 2 pixels wide
                            <br>Fixed some crashes on systems with buggy GPU drivers. Paint.NET will try to revert to
                            software rendering in this case.
                            <br>Fixed a crash on some systems with multiple pen/tablet devices, where some of the
                            devices were claiming the same cursor ID
                            <br>Changed: All binaries are now digitally signed, not just EXEs and the shell extension
                            DLLs (thanks @null54 for the help!)
                            <br>Updated the bundled AvifFileType plugin to version 1.1.23, which fixes an issue with
                            progressive decoding (thanks @null54!)
                            <br>Updated the bundled DDSFileTypePlus plugin to version 1.11.0.0, which now detects files
                            saved with the wrong extension and tries to load the file anyway (thanks @null54!)
                            <br>Updated the bundled WebPFileType plugin to version 1.3.16.0, which fixes the detection
                            of misnamed files (thanks @null54!)
                            <br>
                            <br>
                            <br>paint.net 5.0 - released on January 10th, 2023
                            <br>This is a major update with new features and improvements such as pressure sensitivity
                            for pens and drawing tablets, greatly expanded use of the GPU for effects, adjustments, and
                            tools, and a brand new effect plugin system that includes support for GPU rendering with
                            Direct2D. For a more detailed description of the new features and changes, check out the
                            forum post for this release.
                            <br>New: The app has been updated to run on .NET 7.
                            <br>Changed: Windows 10 (v1809+) or Windows 11 is now required. Windows 7 and 8.1 are no
                            longer supported.
                            <br>Changed: A 64-bit CPU and 64-bit version of Windows are now required. Both AMD/Intel x64
                            and ARM64 are supported. 32-bit x86 is no longer supported.
                            <br>Improved performance: There has been significant optimization work throughout the app
                            and rendering engines to reduce and remove transient allocations, resulting in smoother,
                            faster performance.
                            <br>New: Pressure sensitivity for brush tools (Paintbrush, Eraser, Clone Stamp, Recolor) is
                            now supported for pens and drawing tablets that support Windows Ink.
                            <br>New: The Settings dialog now has a Pen &amp; Tablet section. Currently it has an
                            enable/disable checkbox for Windows Ink.
                            <br>New: Brush tools now support path smoothing, which is enabled by default and can be
                            toggled in the toolbar.
                            <br>New: Brush tools now have a Spacing property in the toolbar.
                            <br>Changed: The Layers and History windows now use the GPU for rendering.
                            <br>Changed: Thumbnails in the Layers window have been made 20% larger.
                            <br>Changed: The image thumbnail list at the top of the main window now uses the GPU for
                            rendering. It has also received some minor improvements in visual styling and quality.
                            <br>Changed: The selection is now rendered using the GPU, which helps with both performance
                            and battery life.
                            <br>New: The brightness of the transparency checkerboard can now be configured in Settings.
                            <br>New: You can now click-and-hold on +/- buttons in the toolbar instead of repeatedly
                            clicking on them.
                            <br>New: Image → Resize now has an ultra-high quality "Adaptive (Best Quality)" option,
                            which is now the default.
                            <br>New: Image → Resize now supports "Lanczos" resampling (it uses 3 lobes).
                            <br>Changed: The "Bilinear" and "Bicubic" options in Image → Resize are now much higher
                            quality. The old "Bilinear" mode has been retained and renamed to "Bilinear (Low Quality)".
                            <br>Removed: The "Super Sampling" mode for Image → Resize has been removed, as it has been
                            superceded by "Adaptive (Best Quality)". It also had some rendering bugs that could not be
                            resolved.
                            <br>New: Image → Apply Embedded Color Profile, which will convert an image to sRGB and then
                            discard the color profile. This helps when working with images that have a color profile so
                            that they look correct in the app and have the same appearance outside of it.
                            <br>Changed: The Line/Curve and Shapes tools now have much higher quality antialiasing.
                            <br>New: The Line/Curve tool now has a Straight mode.
                            <br>New: The Move Selected Pixels tool now uses the GPU when the Bicubic resampling mode is
                            used.
                            <br>New: The Move Selected Pixels tool now has an Anisotropic resampling mode, which uses
                            the GPU for rendering.
                            <br>Changed: The default resampling mode for the Move Selected Pixels tool is now Bicubic if
                            a capable GPU is detected.
                            <br>New: The Settings dialog now has a Graphics section for configuring GPU and hardware
                            acceleration settings.
                            <br>New: Most effects and adjustments have been rewritten to execute on the GPU. A Direct3D
                            11 compatible GPU is required, otherwise CPU rendering will be used.
                            <br>Changed: Effects now run at a higher, smoother framerate. Previously the update speed
                            was limited to 20 frames per second.
                            <br>New: A brand new, modern, high-performance effect plugin system that supports both CPU
                            and GPU effects. GPU effects use Direct2D's effects system ("DirectImage") which is based on
                            a transform graph (aka "nodes"). Custom pixel shaders are also supported.
                            <br>New: Effects that use the new plugin system can now access all of the layers in the
                            current image, along with their metadata (EXIF, XMP, IPTC).
                            <br>New: Effects that use the new plugin system can now render outside of the active
                            selection.
                            <br>New: Plugins that use IndirectUI can now add tabs to their UI.
                            <br>New: Plugins that use IndirectUI can now use a Label control.
                            <br>New: Plugins that use IndirectUI can now set the ShowHeaderLine property to false to
                            clean up how headers look.
                            <br>New: Plugins that use IndirectUI can now set a dropdown control's Multiline property to
                            false to put the label and dropdown on the same line.
                            <br>New: Added a new IndirectUI property collection rule,
                            SetTargetWhenSourceEqualsAnyValueRule, which can be used to implement correlations between
                            dropdowns and sliders (among other things).
                            <br>New: Added a link in the Effects menu to Settings → Plugin Errors if there are any
                            plugin load errors
                            <br>New: On non-English systems, Paint.NET will attempt to auto-localize the submenu names
                            that effect plugins specify. For example: an Italian user will now see just a "Sfocature"
                            sub-menu instead of both "Sfocature" and "Blurs".
                            <br>Changed: Layers → Rotate Zoom, which is technically an effect, now renders using the GPU
                            and has a Quality slider, a Sampling property (Bilinear or Nearest Neighbor), and a Tiling
                            Mode dropdown with options for None, Repeat, and Mirror (the new dropdown replaces the
                            Tiling checkbox).
                            <br>Removed "Preserve Background" from Rotate/Zoom
                            <br>New: Adjustments → Exposure, which uses the GPU for rendering.
                            <br>New: Adjustments → Highlights / Shadows, which uses the GPU for rendering.
                            <br>New: Adjustments → Temperature / Tint, which uses the GPU for rendering.
                            <br>Changed: Adjustments → Brightness / Contrast now uses the GPU for rendering.
                            <br>Changed: Adjustments → Curves's UI now uses the GPU for rendering.
                            <br>Changed: Adjustments → Hue / Saturation now uses the GPU for rendering.
                            <br>Changed: Adjustments → Levels' UI now uses the GPU for rendering.
                            <br>Changed: Adjustments → Posterize now uses the GPU for rendering, and also allows
                            posterization of the alpha channel.
                            <br>Changed: Adjustments → Sepia now uses the GPU for rendering and has an Intensity slider.
                            <br>Changed: Effects → Artistic → Ink Sketch now runs on the GPU and is significantly
                            faster.
                            <br>Changed: Effects → Artistic → Pencil Sketch now runs on the GPU and is significantly
                            faster.
                            <br>New: Effects → Blurs → Bokeh, which uses the GPU for rendering. It uses gamma-correct
                            rendering by default, or you can customize the gamma exponent for artistic/aesthetic
                            preference.
                            <br>Changed: Effects → Blurs → Fragment now uses the GPU for rendering and has improved
                            performance and quality.
                            <br>Changed: Effects → Blurs → Gaussian Blur now has a Quality slider and greatly improved
                            rendering quality. It now uses gamma-correct rendering by default, or you can customize the
                            gamma exponent for artistic/aesthetic preference.
                            <br>Changed: Effects → Blurs → Motion Blur has an Edge Mode property to control how pixel
                            samples outside of the image are determined.
                            <br>Changed: Effects → Blurs → Radial Blur has improved rendering quality, and its Quality
                            slider can now be set between 1.0 and 8.0 in steps of 0.1.
                            <br>Changed: Effects → Blurs → Zoom Blur now uses the GPU for rendering, has improved
                            rendering quality, and a Focus property to control the balance between the foreground and
                            background. It also has a quality slider thar can be set between 1.0 and 8.0 in steps of
                            0.1.
                            <br>Removed Effects → Blurs → Unfocus, which has been replaced by the new Bokeh effect.
                            <br>Changed: Effects → Distort → Bulge now uses the GPU for rendering, has improved
                            rendering quality, and an Edge Behavior property.
                            <br>Changed: Effects → Distort → Crystalize now uses the GPU for rendering and has improved
                            rendering quality.
                            <br>Changed: Effects → Distort → Dents now uses the GPU for rendering, has improved
                            rendering quality, and an Angle property.
                            <br>Changed: Effects → Distort → Frosted Glass now uses the GPU for rendering, has improved
                            rendering quality, a Diffusion property, and a Randomize button.
                            <br>Changed: Effects → Distort → Pixelate now lets you specify a Scale Down and a Scale Up
                            mode (pixelation is implemented by first scaling the image down, and then scaling it back
                            up). This allows you to fine-tune the look of the effect for what you want to achieve.
                            <br>Changed: Effects → Distort → Polar Inversion now runs on the GPU which has greatly
                            improved its performance, and it has improved rendering quality.
                            <br>Changed: Effects → Distort → Tile Reflection now runs on the GPU, has improved rendering
                            quality, and an Edge Behavior property which can produce some really interesting results.
                            <br>Changed: Effects → Distort → Twist now runs on the GPU and has improved rendering
                            quality.
                            <br>Changed: Effects → Noise → Add Noise now runs on the GPU and has a Randomize button. It
                            will not re-randomize on every property change like it used to.
                            <br>New: Effects → Object → Drop Shadow, which uses the GPU for rendering.
                            <br>New: Effects → Photo → Straighten, which uses the GPU for rendering.
                            <br>Changed: Effects → Photo → Glow now runs on the GPU and is significantly faster.
                            <br>Changed: Effects → Photo → Sharpen now runs on the GPU and has been completely rewritten
                            to produce much better results. It also now has a Threshold slider.
                            <br>Changed: Effects → Photo → Soften Portrait now runs on the GPU and is significantly
                            faster.
                            <br>Changed: Effects → Photo → Vignette now runs on the GPU.
                            <br>Changed: Effects → Render → Clouds now runs on the GPU and has a large number of
                            additional blend modes.
                            <br>Changed: Effects → Render → Julia Fractal and Mandelbrot Fractal now run on the GPU and
                            are significantly faster. Depending on your CPU and GPU, you will see a performance
                            improvement between 2x to 100x. You can also now choose a Blend Mode for these effects.
                            <br>Changed: Effects → Render → Turbulence now has a Blend Mode dropdown instead of a Blend
                            checkbox.
                            <br>Changed: Effects → Stylize → Edge Detect has been completely rewritten. Instead of an
                            Angle property, it now has Strength and Blurring sliders, an Algorithm dropdown (Sobel or
                            Prewitt), and an Overlay Edges checkbox.
                            <br>Changed: Effects → Stylize → Emboss now runs on the GPU and is significantly faster.
                            <br>New: IPTC metadata is now preserved, and can be both read and written by FileType
                            plugins. Thanks to @null54 for implementing this!
                            <br>Fixed: 32-bit CMYK images are now correctly imported. They are transformed to 32-bit
                            BGRA sRGB and the color profile is discarded. Thanks to Clinton Ingram (@saucecontrol) for
                            consulting on this!
                            <br>Fixed: If a 24-bit TIFF is opened and then saved as a 32-bit TIFF, it will no longer
                            have incorrect SampleFormat metadata
                            <br>Fixed many long-standing issues with keyboard/mouse focus, whereby tool shortcuts would
                            not work when the mouse was in certain places (e.g. over the Tools or History window)
                            <br>Fixed a rare crash in the canvas rendering code
                            <br>Updated the bundled AvifFileType plugin to version 1.1.22.0 (thanks @null54!)
                            <br>
                            <br>paint.net 4.3.12 - released on August 20th, 2022
                            <br>This is a small update that fixes a few bugs and updates the bundled AVIF and WebP file
                            type plugins.
                            <br>Fixed a bug when using Crop to Selection where the image would scroll away to the corner
                            <br>Fixed a rendering bug in the brush tools that would cause some sections of the brush
                            stroke to be rendered twice, making them darker
                            <br>Added the PdnBaseForm.IsAppThemeDark property so that plugins with custom UI can more
                            easily be dark theme aware
                            <br>Fixed a rare crash in the rendering engine due to a race condition
                            <br>Fixed a crash when using multiple monitors plugged into multiple GPUs from different
                            manufacturers (e.g. AMD vs. NVIDIA), while moving the window between monitors
                            (NotCurrentlyAvailableException)
                            <br>Updated the bundled WebPFileType plugin to v1.3.14.0 (thanks @null54!). See its GitHub
                            releases page for more info.
                            <br>Updated the bundled AvifFileType to v1.1.20.0 (thanks @null54!). See its GitHub releases
                            page for more info.
                            <br>
                            <br>
                            <br>paint.net 4.3.11 - released on May 24th, 2022
                            <br>This is a small update that enables dark themed title bars ("immersive dark mode"), and
                            updates the built-in DDS and WebP plugins.
                            <br>New: Title bars now respect Dark Theme in Windows 10 20H1+
                            <br>Updated the bundled WebPFileType plugin to v1.3.12.0 (thanks @null54!)
                            <br>Updated the bundled DDSFileTypePlus plugin to v1.10.12.0 (thanks @null54!)
                            <br>
                            <br>
                            <br>paint.net 4.3.10 - released on March 9th, 2022
                            <br>This is a hotfix to address an error with Image-&gt;Resize when used with certain image
                            sizes.
                            <br>Fixed an error with Image-&gt;Resize when using Nearest Neighbor resampling with certain
                            image sizes
                            <br>
                            <br>
                            <br>paint.net 4.3.9 - released on March 8th, 2022
                            <br>This is a servicing release that fixes a handful of bugs, and updates the bundled
                            AvifFileType plugin.
                            <br>Added a workaround for a bug in the latest Windows 11 Insider "Dev Channel" build
                            10.0.22567.0 that is causing a lot of crashes. Microsoft has a hotfix coming soon.
                            <br>Fixed a compatibility issue with the Shape Maker plugin that was preventing the ability
                            to open or save shapes
                            <br>Fixed the precision of color channel values for images with transparency when using the
                            Invert Colors or Black and White adjustments. Before, color values were reset to zero if the
                            alpha channel was also zero.
                            <br>Fixed the rendering for Image -&gt; Resize when using Nearest Neighbor. Sampling was off
                            by 0.5 pixels, causing incorrect results. Reported here:
                            https://forums.getpaint.net/topic/118703-incorrectoffset-nearest-neighbor-scaling-when-using-resize-dialog/
                            <br>Fixed a crash in the Quantize effect when Alpha Threshold was set to 0 and the image was
                            completely transparent
                            <br>Updated the bundled AvifFileType to version 1.1.19.0. This updates the AOM version to
                            3.3.0. (thanks @null54!)
                            <br>
                            <br>
                            <br>paint.net 4.3.8 - released on February 16th, 2022
                            <br>This update includes a new Layers -&gt; Toggle Layer Visibility (keyboard shortcut: Ctrl
                            + comma) command, some performance improvements, bug fixes, and a new IndirectUI control for
                            plugins (FolderChooser).
                            <br>New: Layers -&gt; Toggle Layer Visibility menu command (keyboard shortcut: Ctrl + comma)
                            <br>Greatly improved performance for the Line/Curve and Shapes tools
                            <br>Improved performance for the Move Selected Pixels tool when using Bicubic resampling
                            <br>Fixed tooltips not going away when menu items are activated by the keyboard (Effects,
                            Adjustments, and File -&gt; Open Recent)
                            <br>Added a FolderChooser control type for IndirectUI-based plugins (thanks @toe_head2001!)
                            <br>Fixed compatibility for Ed Harvey's FastFX PencilSketch effect plugin
                            <br>Fixed a performance bug in the canvas renderer that was causing tiles to be copied to
                            the GPU more often than necessary. This mostly affected performance when drawing or
                            modifying selections, and when scrolling or zooming.
                            <br>Fixed a small memory leak with the allocations made for Win32 synchronization primitives
                            (critical sections and condition variables)
                            <br>Updated the bundled AvifFileType plugin to verison 1.1.18.0, which fixes some issues
                            with EXIF metadata handling. (thanks @null54!)
                            <br>Updated the bundled WebPFileType plugin to version 1.3.11.0, which fixes some issues
                            with EXIF metadata handling. (thanks @null54!)
                            <br>Updated the bundled DDSFileTypePlus plugin to version 1.10.11.0, which adds support for
                            DXGI_FORMAT_R32_FLOAT. This is used by Bethesda's Creation Kit for Fallout 4. (thanks
                            @null54!)
                            <br>
                            <br>
                            <br>paint.net 4.3.7 - released on January 4th, 2022
                            <br>This is a hotfix for a myriad of major issues when "Translucent windows" is disabled.
                            This was caused by a bug introduced in .NET 6.0.1.
                            <br>Fixed the app being completely broken when "Translucent windows" was disabled. This was
                            caused by a bug introduced in .NET 6.0.1. More discussion here:
                            https://forums.getpaint.net/topic/119185-many-problems-with-436/
                            <br>
                            <br>
                            <br>paint.net 4.3.6 - released on January 3rd, 2022
                            <br>This is a hotfix for a crash in the box filter rendering kernel, which is used to
                            generate mip-maps for the canvas when zoomed out.
                            <br>Fixed a stack overflow in the box filter rendering kernel that could cause hangs or
                            crashes when the zoom level was around 1/8th (12.5%) or 1/32nd (3.125%) for particular image
                            sizes e.g. ((N x 2048) + 16)). Reported here:
                            https://forums.getpaint.net/topic/119180-new-update-is-broken-for-me-435/
                            <br>
                            <br>
                            <br>paint.net 4.3.5 - released on January 3rd, 2022
                            <br>This update includes several important bug fixes, and greatly improves performance.
                            <br>Improved rendering performance for most tools, which are now up to 100% faster (see
                            discussion here: https://twitter.com/rickbrewPDN/status/1477344632404996101)
                            <br>Fixed an issue with the Save Configuration dialog where the OK and Cancel buttons were
                            overlapping on Windows 7 (thanks @toe_head2001 for the fix!)
                            <br>Fixed an issue when saving an image with 257 unique colors at 8-bit color depth when the
                            257th unique color was the last (bottom-right) pixel.
                            https://forums.getpaint.net/topic/119047-error-saving-a-file-seems-related-to-bit-depth-being-at-auto-detect/
                            <br>Fixed an issue where the Layers window buttons were not correctly enabling/disabling
                            after an undo/redo operation.
                            https://forums.getpaint.net/topic/119120-with-only-one-layer-create-layer-and-use-ctrlz-to-undo-delete-layer-button-is-still-enabled/
                            <br>Fixed an issue that was preventing the VTF Plugin from saving multi-layer images
                            correctly, as reported at
                            https://www.reddit.com/r/paintdotnet/comments/rnx11j/help_with_vtf_editing_blend_saving/
                            <br>Fixed an issue when saving images at 1-bit or 2-bit color depth, where sometimes not all
                            colors would be included.
                            https://forums.getpaint.net/topic/119082-saving-png-rounds-a-pixel-with-a-value-of-010101-down-to-000000/
                            <br>Fixed an issue with some IndirectUI plugins that were using customized colors for their
                            sliders
                            <br>Fixed a compatibility issue with TR's Morpher plugin
                            https://forums.getpaint.net/topic/107499-trs-morpher-v1110-march-14th-2016/?do=findComment&amp;comment=589420
                            <br>Fixed a compatibility issue with some of @Ego Eram Reputo's older plugins that were
                            unable to launch help links due to a change in .NET 6
                            <br>
                            <br>
                            <br>paint.net 4.3.4 - released on December 3rd, 2021
                            <br>This update fixes a few legacy plugins (some of which were crashing), a bug in the Color
                            Picker tool, and some minor installation issues.
                            <br>Fixed compatibility with the Spaced Text plugin, which was crashing
                            <br>Fixed a bug with the Color Picker tool, which was sampling from a recently hidden layer
                            when using Image sampling mode
                            <br>Fixed the ability to click URLs in some older plugins (CustomBrushesMini, Shape Maker,
                            Vandermotten Effects, and those based on OptionBasedLibrary)
                            <br>Fixed the incorrect registration of the app in the HKCR\Applications registry key, which
                            was affecting some methods for launching the app
                            <br>Fixed many translations which had updates but that had inadvertently not been
                            incorporated into the app itself
                            <br>Fixed the PROGRAMSGROUP property in the MSI (it was being ignored), which affects custom
                            deployments
                            <br>Fixed the CHECKFORUPDATES property which was missing from the MSI. It still worked, but
                            you had to add it yourself. This only affected MSI-based deployment.
                            <br>
                            <br>
                            <br>paint.net 4.3.3 - released on November 21st, 2021
                            <br>This version has been migrated from .NET 5 to .NET 6, includes 3 new translations, Dark
                            Theme improvements on Windows 10+, and many bug fixes.
                            <br>New: The app has been migrated to .NET 6, which has improved both rendering and startup
                            performance
                            <br>New translation: Catalan (ca)
                            <br>New translation: Corsican (co)
                            <br>New translation: Thai (th)
                            <br>Changed: The /createMsi command for the installer has been removed. Instead, you can now
                            download MSIs directly from the GitHub releases page.
                            <br>Improved various UI controls for Dark Theme, e.g. scrollbars (Win10 v1809+ only)
                            <br>Fixed the way various UI controls look on Windows 11, e.g. buttons and drop-down lists
                            <br>Fixed the View -&gt; Zoom to Window command when using the keyboard shortcut (Ctrl+B),
                            which was resetting instead of toggling the zoom level
                            <br>Improved performance during the "extracting" stage of the installer by migrating away
                            from Nullsoft Scriptable Installer System (NSIS)
                            <br>Reduced the download size on ARM64 by about 33%
                            <br>Fixed a rendering bug in the Dents and Polar Inversion effects, as reported here:
                            https://forums.getpaint.net/topic/118746-paintnet-update-changed-the-way-the-dents-distortion-filter-works-causing-unwanted-artifactsglitches-was-this-an-intended-change/
                            <br>Fixed a memory leak in the selection renderer that was consuming gigabytes of GPU
                            memory, resulting in crashes. Thanks to @Zagna for finding this and testing the fix!
                            https://forums.getpaint.net/topic/118806-paint-crashes-if-you-do-a-selection-glitch-and-then-history-jump-forward/?do=findComment&amp;comment=587772
                            <br>Fixed some GDI object leaks, particularly with the Save Configuration dialog, which
                            would eventually result in a crash. Thanks @rechlin for finding and reporting this!
                            https://forums.getpaint.net/topic/118785-crash-due-to-running-out-of-gdi-objects/
                            <br>Fixed a memory leak in Settings -&gt; Tools. Thanks @otuncelli for finding this!
                            https://forums.getpaint.net/topic/118785-crash-due-to-running-out-of-gdi-objects/#comment-588468
                            <br>Fixed an issue that was preventing new plugins from loading their native DLL
                            dependencies as specified in their .deps.json file
                            <br>Fixed the app crashing after an effect plugin crashes when you choose to restart the app
                            <br>Fixed a crash while drawing a selection, right-clicking on the History window before
                            releasing the left mouse button, and then clicking to redo a history entry, as reported
                            here:
                            https://forums.getpaint.net/topic/118806-paint-crashes-if-you-do-a-selection-glitch-and-then-history-jump-forward/
                            <br>Fixed a text rendering bug in some parts of the UI, mostly in Effects, as reported by
                            @midora over at
                            https://forums.getpaint.net/topic/118866-paintnet-43-footnote-of-indirectui-control-in-filetype-shows-artifacts-after-scrolling/
                            <br>Fixed the "untitled:" file name argument prefix, which was preventing Window Clippings
                            from being able to send screenshot
                            <br>Fixed some registry keys that were not being deleted during uninstall
                            <br>Fixed the PdnRepair utility on Windows 7
                            <br>Fixed some inconsistencies with the MSI as compared to v4.2.16 which were causing
                            problems for some deployments
                            <br>Updated the bundled AvifFileType to v1.1.17.0, courtesy of @null54, which updates the
                            AOM version and fixes a crash when reading large EXIF blocks. See its GitHub releases page
                            for more info.
                            <br>
                            <br>
                            <br>paint.net 4.3.2 - released on October 4th, 2021
                            <br>This is a hotfix for the recently released version 4.3 update.
                            <br>Fixed a hang at app startup on systems using certain locales, such as Thai (th-TH)
                            <br>Improved performance of Settings → Tools, which used to take 6-7 seconds to open. Now it
                            takes about 1 second, thanks to @Bruce Bowyer-Smyth
                            <br>Fixed ReadOnlyBoundToNameValuesRule for IndirectUI-based plugins. It was not
                            initializing correctly, although it would work correctly afterward.
                            <br>
                            <br>
                            <br>paint.net 4.3.1 - released on September 27th, 2021
                            <br>This is a hotfix for the recently released version 4.3 update.
                            <br>Fixed an issue with using Explorer's "Open With" menu on Windows 7, 8.1, and some
                            editions of Windows 10
                            <br>Fixed image thumbnails in Explorer's Details View only having a generic document icon
                            instead of the Paint.NET icon
                            <br>Fixed a spurious, harmless error in Settings → Plugin Errors
                            <br>Fixed a race condition that could cause a crash
                            <br>Fixed not being able to use Ctrl+C to copy text from the Setup Downloader, which is
                            especially important for troubleshooting
                            <br>
                            <br>paint.net 4.3 - released on September 22nd, 2021
                            <br>This version has been migrated from .NET Framework to .NET 5, includes major performance
                            optimizations across the entire app, and adds native support for ARM64 devices such as the
                            Microsoft Surface Pro X.
                            <br>New: The app has been migrated to .NET 5, and performance has been greatly improved as a
                            result.
                            <br>New: ARM64 is now natively supported, which improves performance on devices such as the
                            Surface Pro X.
                            <br>New: .NET no longer needs to be installed on the system because the app now uses
                            self-contained deployment.
                            <br>New: Portable ZIPs are now available. Please note that portable installations do not
                            currently update automatically.
                            <br>Improved performance of most effects and other compute-intensive tasks by about 20% on
                            average, due to .NET 5's improved code generation (JIT).
                            <br>Improved startup performance for the Microsoft Store release. Previously, .NET
                            Framework's NGEN was unavailable for Store apps, but now .NET 5 enables self-contained
                            deployment along with ReadyToRun + crossgen, which serves the same purpose.
                            <br>Improved performance: Many areas of the app have been optimized to use SIMD (SSE2/3/4.1,
                            AVX2) on x86/x64:
                            <br>Drawing on an image with a large number of layers is faster
                            <br>Drawing with the Gradient Tool's alpha mode is faster
                            <br>Drawing with the Recolor tool is faster
                            <br>Drawing with the Eraser or Clone Stamp tool is faster when using a color whose alpha
                            value is less than 255
                            <br>Drawing with the Overwrite blend mode is faster
                            <br>Drawing with the Shapes tool is faster, due to improved compositing performance
                            <br>Drawing with a brush tool without antialiasing is faster
                            <br>Tile compression has lower overhead due to being optimized for SSE2 and AVX2
                            <br>Working with complex selections is faster
                            <br>Many other optimizations all throughout the application and rendering engine
                            <br>Improved performance of loading custom Shapes by ~16x on 2nd and subsequent app starts.
                            <br>Improved performance of the Magic Wand tool by a substantial amount.
                            <br>Improved performance of the Paint Bucket tool by a substantial amount.
                            <br>Improved performance of the Paint Bucket when changing the color or certain other
                            toolbar settings by not recalculating the stencil buffer for the filled area. Changes should
                            now be visible immediately.
                            <br>Improved performance of Polar Inversion by 3x, mostly as a corollary to fixing a bug
                            that was causing hangs, and a little bit due to .NET 5.
                            <br>Improved performance on systems without HyperThreading by reserving 1 core for the UI.
                            Performance is also improved on systems with it by utilizing more of the logical cores.
                            <br>Improved performance while installing or updating the app, due to no longer needing the
                            "Optimizing performance for your system" stage (NGEN has been replaced with ReadyToRun via
                            crossgen).
                            <br>Improved memory usage when custom shapes are installed so they don't litter the heap
                            with hundreds of thousands of boxed value types (e.g. floats and points).
                            <br>Improved selection antialiasing quality by using a 4x4 super sampling filter instead of
                            a 3x3 super sampling filter. The code has also been optimized to use SSSE3 on x86/x64.
                            <br>Improved: Effect and File Type plugins can now be organized into folders. The plugin
                            loader will recursively search for DLLs up to 1 folder deep.
                            <br>Fixed a bug when saving with "Auto Detect" bit-depth which was causing fidelity loss on
                            some images that already had 256 colors or less. This was reported here:
                            https://forums.getpaint.net/topic/118401-images-already-with-256-or-fewer-colors-being-dithered-when-saved-with-palette/
                            <br>Fixed: There were some issues with zooming in/out using the keyboard, where the
                            anchoring point was not calculated correctly, causing the canvas to drift in the wrong
                            direction.
                            <br>Fixed the inability to use middle-mouse panning after using a selection tool and
                            pressing delete before releasing the mouse button.
                            <br>Improved: Plugins are now loaded into isolated AssemblyLoadContexts, which improves
                            stability and resiliency to various problems with versioning, loading dependencies, plugin
                            bugs, and incorrect plugin installation.
                            <br>Fixed a crash when trying to draw a fixed-size rectangle selection that was larger than
                            the image.
                            <br>Fixed a bug with the Tolerance slider where both 58% and 59% would be displayed as 58%,
                            due to a rounding issue. The correct value was actually being used, it just wasn't being
                            displayed correctly.
                            <br>Added a /disablePlugins command-line argument to aid in troubleshooting various issues
                            with app startup and incorrect plugin installation.
                            <br>New: Additional directories can now be specified for plugin discovery, which (e.g.)
                            enables the use of OneDrive for storing plugins. See here for more info:
                            https://forums.getpaint.net/topic/118583-feature-request-set-custom-app-files-plugins-folder/?do=findComment&amp;comment=586013
                            <br>Note that this does not work with the portable version of the app, but you can install
                            plugins next to the app so it isn't necessary.
                            <br>Updated the bundled AvifFileType plugin to v1.1.15.0, courtesy of @null54, which
                            includes support for multi-layer AVIF files, and adds native support for ARM64. See the
                            project's GitHub Releases page for more information.
                            <br>Updated the bundled DdsFileTypePlus plugin to v1.10.10.0, courtesy of @null54, which
                            adds native support for ARM64. See the project's GitHub Releases page for more information.
                            <br>Updated the bundled WebPFileType plugin to v1.3.7.0, courtesy of @null54, which adds
                            native support for ARM64. See the project's GitHub Releases page for more information.
                            <br>Changed: FileType.IsReflexive() is now deprecated via [Obsolete], and is no longer
                            honored. However, the Save Configuration dialog will no longer try to generate previews for
                            FileTypes that do not specify any file extensions for loading, which is what this method was
                            being used for.
                            <br>Known Issue: Due to crashing, GPU accelerated effects (Gaussian Blur, Motion Blur,
                            Radial Blur) on ARM64 will actually use the CPU for rendering.
                            <br>
                            <br>paint.net 4.2.16 - released on April 21st, 2021
                            <br>This updates fixes and optimizes palette generation when saving at 8-bit depth or less,
                            and also fixes any remaining issues with using "Auto-detect" for bit-depth. A new effect,
                            Quantize (in the Effects -&gt; Color menu), has been added, some bugs have been fixed, and
                            bundled file type plugins have been updated.
                            <br>New: Effect -&gt; Color -&gt; Quantize, which applies palette reduction to 256 colors or
                            less, along with dithering. This is the same algorithm used when saving images at 8-bit
                            color depth or lower.
                            <br>Fixed and improved palette generation when saving at 8-bit color depth or less
                            <br>Greatly optimized performance of palette generation and image quantization
                            <br>Added option to choose between Octree (default) and Median Cut algorithms for palette
                            quantization when saving at 8-bit color depth or less
                            <br>Fixed a crash in Move tools when the selection was 0-width and/or 0-height
                            <br>Added tooltips w/ shortcut keys to the Tools dropdown in the toolbar
                            <br>Fixed IndirectUI ColorWheel rendering (thanks @toehead2001!)
                            <br>Fixed a crash in the Text tool when using Ctrl+(Left,Right,Backspace,Delete) (thanks
                            @Bruce Bowyer-Smyth!)
                            <br>Changed: New layers are now filled with #00000000 instead of #00FFFFFF
                            <br>Fixed a crash when working with selections (OutOfMemoryException)
                            <br>New: Effects can now access the Document's DPI via
                            EffectEnvironmentParameters.DocumentResolution
                            <br>Fixed drawing of the color palette in the Colors window when using some non-standard DPI
                            scaling settings (e.g. 1.15x)
                            <br>Fixed a crash when using EdHarvey's Threshold plugin
                            <br>Fixed the return value from PdnRegion.GetBoundsInt() so it's not anchored at (0,0)
                            unless it should be
                            <br>Fixed premultiplied-to-straight color conversion on some code paths (thanks @null54!)
                            <br>Updated bundled AvifFileType plugin to v1.1.11.0, which includes performance
                            optimizations and bug fixes. See its GitHub releases page
                            (https://github.com/0xC0000054/pdn-avif/releases) for more info.
                            <br>Updated bundled DDSFileTypePlus plugin to v1.10.9.0, which uses an updated version of
                            DirectXTex (2021-04-06).
                            <br>
                            <br>paint.net 4.2.15 - released on January 24th, 2021
                            <br>This is a small update that improves some quality-of-life issues, and fixes some
                            important crashes due to mishandling of some non-fatal DirectX errors.
                            <br>New: "Tolerance Alpha Mode" toggle button added to the toolbar for the Magic Wand, Paint
                            Bucket, and Recolor tools. This permits switching the algorithm for color comparison between
                            premultiplied (default) and straight. "Straight" will distinguish between transparent pixels
                            with different color values, whereas premultiplied will see them as equivalent.
                            <br>New: Holding Ctrl while using the Color Picker tool will sample from the merged image
                            (vs. just the current layer)
                            <br>New: The file name in the title bar will now have a prepended asterisk when it has
                            unsaved changes
                            <br>Changed: The image close 'X' button can now be clicked for images that are not currently
                            active
                            <br>Changed: In the Text tool, Ctrl+(Backspace, Delete, Arrow Keys) has been improved to
                            work more like Microsoft Word. Thanks to @Bruce Bowyer-Smyth for the patch!
                            <br>Fixed: The Rectangle Select tool, when used to draw a constrained, fixed ratio, or fixed
                            size selection, will now correctly clamp the rectangle to be within the canvas
                            <br>Fixed: Layers -&gt; Move Layer Up/Down/Top/Bottom was not working for images with fewer
                            than 3 layers
                            <br>Fixed: Edit -&gt; Erase Selection will now fill with transparent black (#00000000)
                            instead of transparent white (#00FFFFFF)
                            <br>Fixed: Custom Shapes will now be displayed in a consistently sorted order
                            <br>Fixed: ".pdnSave" ghost files should no longer linger when saving to the desktop. This
                            was due to a bug in Windows and File Explorer.
                            <br>Fixed crashes due to DXGI/Direct3D "lost device" or "device removed" errors that can
                            happen for various reasons (duck/undock, driver update, low memory, etc.)
                            <br>New: Plugins can now use the IArrayPoolService, a wrapper around .NET's ArrayPool, to
                            optimize their array allocations
                            <br>Updated bundled AVIF FileType Plus to v1.1.6. See the pdn-avif releases page on GitHub
                            (https://github.com/0xC0000054/pdn-avif/releases) for more information.
                            <br>
                            <br>paint.net 4.2.14 - released on October 23rd, 2020
                            <br>This updates adds full support for AV1 (*.avif) images, includes many optimizations to
                            improve performance, CPU usage, and memory usage, and also has several important bug fixes.
                            <br>New: AV1 (*.avif) images can now be saved (not just opened), due to bundling of
                            @null54's AvifFileType plugin (v1.1.4.0). Installation of Microsoft's codec from the
                            Microsoft Store is no longer necessary, which means this also works on Windows 7 and 8.1.
                            <br>Improved performance and memory usage in the canvas rendering engine, especially when
                            working with large images or images with many layers. This is most noticeable when scrolling
                            and zooming.
                            <br>Improved CPU usage when a selection is active and when GPU accelerated rendering is
                            disabled
                            <br>Improved CPU/GPU usage when a selection is active but the app is not (the animation is
                            disabled)
                            <br>Reduced memory usage when working with images that have regions of solid color
                            <br>Fixed the Magic Wand and Paint Bucket tools so that they do calculations in the
                            premultiplied alpha color space. This ensures that transparent colors (alpha=0) with
                            different RGB values are treated as equal, and do not create borders.
                            <br>Fixed the Move Selected Pixels tool so that it fills the uncovered region with 0
                            (transparent), instead of a transparent version of the secondary color.
                            <br>Fixed: Backspace now works correctly in the Colors form: it does not execute Edit → Fill
                            Selection
                            <br>Fixed an issue where saving an image at 4-bit color depth (usually pixel art) was using
                            an incorrect palette (reduced color count/quality). This was due to a bug in Windows Imaging
                            Component (WIC).
                            <br>Greatly improved performance when saving images at 8-bit color depth
                            <br>Fixed an issue where very large images (e.g. 50000 x 50000 px) couldn't be saved at
                            indexed bit-depths (8-bit or less) due to a bug in Windows Imaging Component (WIC). More
                            information on the forum:
                            https://forums.getpaint.net/topic/116950-error-when-saving-a-big-file/
                            <br>Fixed an issue where BMP images couldn't be loaded if they had the .PNG extension
                            (there's an Android screenshot utility out there which does this ...)
                            <br>Improved: Ellipse Selection Tool's now tessellates at a higher resolution, resulting in
                            smoother circles at small sizes
                            <br>Fixed a rare crash in the Gradient tool ("The tool must be in the Drawing state ...")
                            <br>New: Added a list of the DLLs that are loaded into the process on the Settings →
                            Diagnostics page. This is to help troubleshooting scenarios.
                            <br>Fixed an issue with copying large images to the clipboard: if an image would take up
                            more than 4GB, it could not be copied because the DIB and DIBV5 formats cannot be larger
                            than that. Now, the DIB and DIBV5 formats are not placed on the clipboard if this happens.
                            <br>Fixed an issue with Effect plugin tooltips which was preventing the menu item from being
                            easily clicked (thanks @toe_head2001 for the fix!)
                            <br>Fixed an issue that was preventing Effect configuration dialogs from working correctly
                            in the Visual Studio designer (thanks @toe_head2001 for the fix!)
                            <br>Added diagnostics information to most error dialogs. This is to help with
                            troubleshooting.
                            <br>Fixed: Scanning will now apply the DPI (resolution) from the scanner to the image, if
                            possible
                            <br>Updated bundled DdsFileTypePlus plugin to v1.10.7.0. See the pdn-ddsfiletype-plus change
                            log on GitHub for more information. Thanks @null54!
                            <br>
                            <br>paint.net 4.2.13 - released on August 4th, 2020
                            <br>This update adds some additional low-bit-depth choices to several file types (PNG, BMP,
                            TIFF), and fixes some bugs.
                            <br>New: Added 2-bit per pixel support when saving as PNG
                            <br>New: Added 1-bit per pixel support when saving as PNG, BMP, and TIFF
                            <br>Fixed low-bit-depth saving quality (8-bit, etc.), as it would sometimes produce very bad
                            results (e.g. only using 64 colors instead of 256)
                            <br>Fixed: Resizing an image at very large sizes (e.g. 32K pixels to 64K pixels) would fail
                            due to an arithmetic overflow
                            <br>Fixed: Sometimes recently saved images would not have an updated thumbnail in File
                            Explorer unless/until its window was manually refreshed
                            <br>Fixed: Sometimes saving an image to a network share would not work
                            <br>Updated bundled DDSFileTypePlus plugin to version 1.10.4.0, which fixes an issue when
                            loading and saving images using the sRGB color space. This issue was reported here. Thanks
                            @null54!
                            <br>
                            <br>paint.net 4.2.12 - released on May 29th, 2020
                            <br>This is a hotfix for a few important issues that have come to light with the 4.2.11
                            release.
                            <br>Fixed an error that was preventing some old PDN images from loading (reported here:
                            https://forums.getpaint.net/topic/116501-error-opening-older-pdn-files/)
                            <br>Fixed a crash in the new selection outline renderer (due to misaligned
                            Push/PopAxisAlignedClip calls)
                            <br>Changed saving to use the ReplaceFile Win32 API, which improves its compatibility
                            <br>Fixed an EndOfStreamException error that prevented some JPEGs from opening (thanks
                            @null54 for the fix!)
                            <br>
                            <br>paint.net 4.2.11 - released on May 20th, 2020
                            <br>This update adds XMP metadata support, 3 new translations, some UI improvements, and
                            several bug fixes.
                            <br>New: XMP metadata is now preserved for supported file types (PDN, JPEG, PNG, TIFF, JPEG
                            XR, HEIC, AVIF, WEBP)
                            <br>New: Belarusian (be) translation
                            <br>New: Greek (el) translation
                            <br>New: Slovenian (sl) translation
                            <br>New: Added a right-click context menu to the image thumbnail/tab. It contains commands
                            for Copy Path, Open Containing Folder, Save, Save As, and Close.
                            <br>New: The items in the File -&gt; Open Recent menu now have a tooltip with the full file
                            path for the image
                            <br>Changed: The selection outline animation is now smoother (2x the framerate)
                            <br>Fixed: Saving with the HEIC file type is no longer limited to a max Quality value of 90.
                            This limitation was in place because of a crash due to heap corruption, which no longer
                            happens.
                            <br>Fixed: The NVIDIA sharpening setting will no longer cause trippy distortions in the
                            canvas area
                            <br>Fixed an issue with loading very small TGA images, first reported here:
                            https://forums.getpaint.net/topic/116100-tga-rle-truecolor-1x1-image-failed-to-load/. Thanks
                            @null54 for the fix!
                            <br>Fixed: Error dialogs when opening images now consistently show the file path
                            <br>Fixed a PropertyNotFoundException error message when saving JPEG images with a
                            particular ordering of metadata. This was due to a bug in Windows 7's WIC JPEG codec. First
                            reported here: https://forums.getpaint.net/topic/116079-jpg-cant-save-some-file/
                            <br>Fixed clipped text rendering in the Curves adjustment dialog in some non-English
                            translations.
                            <br>Fixed a crash when running the app with a DPI scaling setting of 500%
                            <br>Fixed a crash that would sometimes happen when running effects with very small
                            selections
                            <br>Fixed some IndirectUI controls not honoring their default values if also initialized in
                            read only (disabled) mode. Thanks @BoltBait for the fix!
                            <br>Fixed a memory leak in the effect system that was causing 1 orphaned thread per effect
                            invocation
                            <br>Changed: Removed the use of NTFS Transactions, which was causing trouble with OneDrive.
                            Microsoft has also deprecated this technology.
                            <br>New: Added /openCrashLogFolder command-line argument. This is intended for simplifying
                            troubleshooting workflows.
                            <br>New: Added /forceUpdateCheck command-line argument. This is intended for troubleshooting
                            scenarios to simplify acquiring the latest version, e.g. "just run
                            paintdotnet:/forceUpdateCheck" instead giving a longer list of buttons to click on.
                            <br>Updated WebPFileType plugin to version 1.3.4.0, which adds XMP metadata support. Thanks
                            @null54!
                            <br>Updated DDSFileTypePlus plugin to version 1.10.3. This fixes an issue with saving in the
                            A1R5G5B5, A4R4G4B4, and R5G6B5 formats, and adds support for reading files that use a
                            'BC7\0' FourCC. Thanks @null54!
                            <br>
                            <br>paint.net 4.2.10 - released on February 13rd, 2020
                            <br>This small update fixes a few important bugs, most notably with installations that
                            directly use the MSI file for deployment (e.g. AD/GPO).
                            <br>Fixed: Installations that directly use the MSI (e.g. AD/GPO deployments) no longer need
                            to run the repair process immediately after installation. Some important DLLs were not being
                            updated because while their assembly version was different, their file version was
                            unchanged, so Windows Installer incorrectly skipped over them. Click here for more
                            information.
                            <br>Fixed: Loading an image with an enormous photoshop:DocumentAncestors node in the XMP
                            metadata will no longer hang the app
                            <br>Fixed a rare crash in the auto-updater UI related to font initialization
                            <br>Improved performance when clicking OK on an effect or adjustment dialog that has already
                            completed part of its rendering
                            <br>
                            <br>paint.net 4.2.9 - released on January 31st, 2020
                            <br>This updates improves performance and significantly reduces memory usage, adds two new
                            translations, and fixes a number of small issues.
                            <br>Reduced overall memory usage (commit size) by up to 1/3rd by eliminating the per-image
                            scratch buffer
                            <br>Greatly improved performance when finishing actions of most tools by employing a shared
                            cache between the render and commit code paths
                            <br>Reduced memory usage when working with many tools by consolidating homogenous tiles
                            (those that are comprised of a single color value)
                            <br>Significantly improved performance of most history actions (commit, undo, redo) by
                            switching from NTFS compression to multithreaded LZ4 compression for history files
                            <br>Significantly improved performance of undo/redo with very complex selections (e.g. from
                            the Magic Wand tool)
                            <br>Improved performance of Image -&gt; Flatten (also affects flattening when saving)
                            <br>Improved performance of the Invert Colors and Desaturate adjustments by disabling
                            hardware acceleration for them (too much overhead in copying tiles to the GPU for such
                            trivial rendering kernels)
                            <br>Improved performance when saving by moving thumbnail rendering for the File -&gt; Open
                            Recent menu to a background thread
                            <br>Reduced memory usage when printing, and removed a rare crash that was related to its use
                            of the (now removed) scratch buffer
                            <br>Improved performance of effect rendering when a complex selection is active (improved
                            caching)
                            <br>New: Added a "busy spinner" to the canvas when using the Magic Wand and Paint Bucket
                            tools
                            <br>New translation: Hebrew (HE)
                            <br>New translation: Slovak (SK)
                            <br>Fixed a really goofy crash that required drawing with the paintbrush and, without
                            letting go of the mouse button, moving the mouse into the toolbar and then using the mouse
                            wheel to change the brush width
                            <br>Fixed a layout bug with the image list button
                            <br>Fixed an error that prevented saving some images as JPEGs if they had EXIF Interop
                            metadata (PropertyNotFoundException)
                            <br>Fixed a crash when running on a CPU that supports AVX but with an OS that is configured
                            to not support it (via bcdedit /set xsavedisable 1)
                            <br>Fixed a crash when pressing the spacebar after switching to a tool but before it has
                            received any mouse input events
                            <br>Fixed a rare crash when opening the Levels adjustments with certain types of selections
                            <br>Fixed a crash when checking for updates with an expired alpha/beta build
                            <br>Fixed a crash (FileLoadException) when DLLs are not updated correctly by the updater
                            <br>Updated WebPFileType plugin to version 1.3.2 (thanks @null54!)
                            <br>Updated DDSFileTypePlus plugin to version 1.9.9. This adds support for X8B8G8R8 and
                            R8G8B8 formats, and fixes a visual glitch when previewing cube maps in some formats. (thanks
                            @null54!)
                            <br>
                            <br>paint.net 4.2.8 - released on December 3rd, 2019
                            <br>This small update fixes a few pressing bugs, particularly for touch and pen input.
                            <br>Fixed: Pinch-to-zoom was not working when using a touch screen (regression in 4.2.6)
                            <br>Fixed: Spacebar panning was not working when using a pen/stylus (regression in 4.2.6)
                            <br>Fixed: EXIF metadata with non-ASCII characters is now preserved correctly
                            <br>Fixed a crash that can happen when the Microsoft Store version of the app is closed for
                            an update
                            <br>Added /repair command-line argument, which will run PdnRepair.exe. This makes it easy to
                            use Start -&gt; Run -&gt; paintdotnet:/repair so you don't have to go fishing for the
                            installation directory.
                            <br>
                            <br>paint.net 4.2.7 - released on November 25th, 2019
                            <br>This hotfix addresses a crash at startup that was happening on some systems.
                            <br>Fixed a crash at startup (FileLoadException) due to 1) the stub for System.Runtime.dll
                            not being updated, and 2) the rigid version binding policy that prevented the older version
                            from working in its stead (which would've been fine in this case).
                            <br>
                            <br>paint.net 4.2.6 - released on November 21st, 2019
                            <br>This update is focusing on some important fixes and performance improvements, and
                            getting some infrastructure ready for future releases so that pens and tablets with pressure
                            sensitivity can be fully supported (planned for v4.3).
                            <br>Improved the input handling systems to use WM_POINTER, which enables glitch-free drawing
                            when using a pen or stylus (e.g. Surface Pen, Wacom/Ugee tablet) (see here:
                            https://forums.getpaint.net/topic/113173-the-first-5mm-of-a-freehand-line-are-straight-when-using-a-tablet/
                            ). This will also be the basis for adding pressure sensitivity in a future release (v4.3).
                            <br>Added a "Native pointer input" setting if a "pointer" device is available (pen, tablet,
                            touch screen). Disabling this will cause any pointer device to be emulated as a mouse, which
                            may be more compatible but at the cost of smoothness. Pointer devices are listed in Settings
                            -&gt; Diagnostics.
                            <br>Removed the "Fluid mouse input" setting because the use of GetMouseMovePointsEx() has
                            been removed (it's a very buggy and broken API). This finally fixes a number of weird issues
                            related to erratic or "scribbly" drawing.
                            <br>Improved performance of Move Selected Pixels, Shapes, and Gradient tools when releasing
                            the mouse button at the end of drag-and-drop gesture. Previously, anything rendered between
                            the last mouse "move" and "up" events was re-rendered, resulting in the appearance of a
                            delay/lag.
                            <br>Greatly improved performance of layer thumbnails when switching between images
                            <br>Improved: The image list at the top can now be scrolled by clicking the arrow buttons
                            and holding the mouse down, just like a regular scroll bar button. (Previously you had to
                            click repeatedly). This improves usability, but was also noted as being important for
                            accessibility.
                            <br>Improved: Smooth scrolling animations have been removed from the image list and layers
                            list due to them just not working very well.
                            <br>Improved window chrome/theming when the app is running in Remote Desktop on Windows 10
                            <br>Changed: The size of the default/initial image ("Untitled") is now scaled exactly by
                            system DPI setting (previously scaled by integer/floor of DPI setting). So at 150% DPI
                            scaling this image will now be 1200x900 instead of 800x600.
                            <br>Fixed some high-DPI layout bugs with the Layer Properties dialog, while also preparing
                            this UI for future additions
                            <br>Fixed a crash (OutOfVideoMemoryException) on systems with hybrid GPU setups that are
                            configured wrong. This seems to be a bug in Windows and DirectX. A "hybrid GPU" setup is an
                            Intel iGPU or AMD APU paired with a discrete GPU in a laptop.
                            <br>Improved handling of the dreaded "NoHardwareDeviceException" crash: The user will be
                            notified of how to fix this. It happens only on 2nd generation Intel Core systems with
                            NVIDIA "Optimus" GPUs (GeForce or Quadro) when the NVIDIA Control Panel is set to force apps
                            (or just Paint.NET) to use the NVIDIA GPU. This is a bug in the NVIDIA driver and/or in
                            DirectX.
                            <br>Fixed images being pasted incorrectly from Outlook 2016/365. This is actually a bug in
                            Outlook: it puts PNGs on the clipboard that are arbitrarily cropped and scaled for some
                            reason, and specifies they are the preferred format to use when pasting. This completely
                            boggles my mind, it's just really weird, I can't imagine why it's done this way.
                            <br>Fixed some clipboard image handling for plugins (regular Copy/Paste is unaffected)
                            <br>Changed: SSE2 is now required for 32-bit/x86 systems (prevously, only SSE was required).
                            See blog post:
                            https://blog.getpaint.net/2019/10/14/paint-net-v4-2-6-will-require-sse2-on-32-bit-x86/
                            <br>Updated bundled WebPFileType plugin to v1.3.1.0 (thanks @null54!)
                            <br>Updated bundled DDSFileTypePlus plugin to v1.9.8.0 (thanks @null54!)
                            <br>
                            <br>paint.net 4.2.5 - released on October 1st, 2019
                            <br>This update adds WebP (*.webp) support and fixes a few important bugs.
                            <br>New: WebP images are now supported due to bundling @null54's excellent WebPFileType
                            plugin (v1.3.0.0)
                            <br>Fixed: Pasting images from Firefox's "Take a Screenshot" feature was resulting in
                            swapped red and blue channels due to mishandling of DIB_V5 clipboard data using the BI_RGB
                            value for bV5Compression (thanks @null54 for the fix!)
                            <br>Fixed crash at startup (for both app and installer) on Windows "N" editions due to
                            missing mfplat.dll (Media Foundation Platform)
                            <br>Updated bundled DDSFileTypePlus plugin to v1.9.7.0
                            <br>
                            <br>paint.net 4.2.4 - released on September 20th, 2019
                            <br>This hotfix addresses some crashes and hangs that were happening when saving DDS images
                            in certain formats.
                            <br>Fixed a hang, which sometimes also resulted in a crash, when saving DDS images in
                            certain formats (e.g. BC1/DXT1)
                            <br>Improved: Reduced CPU usage in the COM interop system, which should help reduce overall
                            power consumption
                            <br>
                            <br>paint.net 4.2.3 - released on September 19th, 2019
                            <br>This hotfix addresses an issue that was preventing DDS images from working on some
                            systems.
                            <br>Fixed: A missing DLL, vcomp140.dll, was preventing the bundled DDSFileTypePlus plugin
                            from loading on some systems
                            <br>
                            <br>paint.net 4.2.2 - released on September 18th, 2019
                            <br>This update adds AV1 (*.avif) loading support, significantly improves DirectDraw Surface
                            (DDS) support, adds 4-bit saving for PNG, BMP, and TIFF, fixes several bugs, and optimizes
                            startup time.
                            <br>New: AV1 (*.avif) images can now be opened (saving is not supported). Windows 10 v1809+
                            and Microsoft's AV1 Codec are required (download:
                            https://www.microsoft.com/p/av1-video-extension-beta/9mvzqvxjbq9v )
                            <br>New: DirectDraw Surface (*.dds) support has been greatly improved due to bundling
                            @null54's DDSFileTypePlus v1.9.6.0 plugin. All DX10/DX11 formats should now be supported
                            (e.g. BC4, BC5, BC6H, BC7), and encoding (saving) will make use of the GPU to greatly
                            improve performance. Note that it's no longer necessary to use the ".dds2" file extension.
                            <br>New: 4-bit saving is now supported for PNG, BMP, and TIFF
                            <br>New: The palette selection menu will now indicate which palette is currently active
                            (thanks @null54 for the implementation!)
                            <br>Improved: The maximum image size is now 262,144 x 262,144 pixels, up from 65,535 x
                            65,535 pixels. This is mostly for accommodating very tall or very wide images.
                            <br>Improved: Startup performance has been improved for multi-core CPUs
                            <br>Improved: Startup performance has been improved when a lot of custom shapes are
                            installed
                            <br>Fixed: EXIF metadata of type Float and Double are now supported. This ensures GeoTIFF
                            metadata is preserved.
                            <br>Fixed: Opening an image should no longer flicker due to the transparency checkerboard
                            being drawn first
                            <br>Fixed: TGA images that are 16-bit with 1-bit alpha with a zero'd out alpha channel are
                            now treated as opaque. This allows images from 5CC Map Maker (for Close Combat modding) to
                            work. Thanks @null54 for the fix!
                            <br>Fixed: JPEG XR's file extensions (*.jxr, *.wdp, *.wmp) are now registered with Explorer
                            <br>Fixed: Pasting images that use RGB pixel ordering should now work (this affects
                            PaintTool SAI)
                            <br>Fixed a crash when manually typing in a very large number for the zoom level in the
                            status bar
                            <br>
                            <br>paint.net 4.2.1 - released on August 7th, 2019
                            <br>This update addes JPEG XR file type support and fixes several important issues and
                            crashes.
                            <br>New: JPEG XR file type support (Windows 8.1+ required)
                            <br>Fixed: Holding Ctrl when dragging a selection with Move Selected Pixels will again leave
                            a copy behind (but only with the mouse)
                            <br>Fixed crashes when saving DDS images
                            <br>Fixed VTF file type plugin. It was not working in 4.2 except for images that were an
                            exact power-of-2 size on each dimension.
                            <br>Fixed: .BMP files can be opened even if they're not actually BMP images (they still need
                            to be a valid WIC-supported file type such as PNG, JPEG, etc.)
                            <br>Fixed very bad performance when opening large images with embedded rotation metadata
                            <br>Fixed various crashes, such as when using File-&gt;New or Image-&gt;Resize, that
                            sometimes happened if the previous update needed a reboot but either 1) it didn't tell you
                            that, or 2) it did but you didn't reboot
                            <br>Fixed the problem that was causing the need for the aforementioned reboot in the first
                            place (string resources file was locked by the thumbnail provider shell extension)
                            <br>Fixed: Text tool will no longer draw tiny text when an image uses dots-per-centimeter
                            instead of dots-per-inch
                            <br>Fixed menu ordering of effect plugins that have duplicate names
                            <br>Fixed: The mouse wheel may now be used to scroll the Palettes menu in the Colors window
                            (thanks @AndrewDavid for the suggestion and @toe_head2001 for the fix!)
                            <br>Fixed metadata handling that was preventing some images with EXIF tag 330 from being
                            able to load
                            <br>Fixed metadata preservation for old images that pad EXIF string values with null
                            terminators
                            <br>Fixed title bar text color when using certain custom accent colors in Windows 10
                            <br>Fixed title bar accent color when Tablet Mode is enabled
                            <br>
                            <br>paint.net 4.2 - released on July 13th, 2019
                            <br>This is a big update that focus on adding HEIC file format support, fixing performance
                            with very large images, and upgrading and modernizing the functionality of many existing
                            file types (JPEG, PNG, BMP, GIF, and TIFF). Many other quality of life issues have also been
                            addressed or fixed.
                            <br>New: Support for loading and saving HEIC images (Windows 10 v1809+ and codec
                            installation is required). Please note that the "Quality" slider when saving is limited to a
                            value of 90 (out of 100) while Microsoft investigates and fixes a crash in their codec.
                            <br>New: Keyboard shortcuts for changing the current layer. You can see these in the Layers
                            menu with the "Go to ..." commands. Alt+PgUp/PgDown will go to the layer above/below, and
                            Ctrl+Alt+PgUp/PgDown will go to the top/bottom layer.
                            <br>Fixed: Optimized rendering engine to remove huge lag spikes (30+ seconds) when zooming
                            or panning very large images (e.g. 32K x 32K pixels).
                            <br>Improved: BMP now supports saving in 32-bit (with alpha!) and 8-bit indexed.
                            <br>Improved: Added DIB and RLE file extensions to the BMP file type.
                            <br>Improved: PNG, JPEG, and TIFF now support loading and saving of much larger images.
                            <br>New: PNGs can now be saved as "interlaced".
                            <br>Improved: JPEG now has configuration for the chroma subsampling mode (4:4:4, 4:2:2, and
                            4:2:0). The default is now 4:2:2 instead of the unconfigurable 4:2:0 of older versions. This
                            may result in larger file sizes, but higher quality, as compared to previous versions.
                            <br>Improved: TIFF now supports saving at 24-bit and 8-bit color depths.
                            <br>Improved performance of saving for file types where "Auto" bit-depth is supported but is
                            not the current choice.
                            <br>Improved temporary memory usage when saving images at 8-bit color depth.
                            <br>Improved: TGA images now load about 4x faster (thanks @null54!)
                            <br>Fixed: 8-bit TGA images should now load correctly (thanks @null54 for the fix!)
                            <br>Fixed: Some 32-bit TGA images were showing up as completely transparent due to their use
                            of an obscure alpha channel type (thanks @null54 for the fix!)
                            <br>Improved: Added error reporting to the Save Configuration dialog. Instead of just saying
                            "Preview: (error)", you'll also get the standard error dialog that includes the exception
                            which can used for troubleshooting.
                            <br>Fixed a number of performance issues in the Save Configuration dialog. Especially with
                            large images, it should now be much faster to change options and to click OK/Cancel.
                            <br>Fixed flickering in the Save Configuration dialog when changing options.
                            <br>Fixed: Windows Explorer thumbnails for some image types (PDN, DDS, TGA) were not
                            rendering their alpha (transparency) correctly, resulting in color skew. You may not see the
                            effect of this fix for a particular image until that image is resaved or you clear
                            Explorer's thumbnail cache.
                            <br>Fixed: Mouse cursors now scale appropriately for non-integer UI scales (e.g. 125% or
                            175%)
                            <br>Fixed: AltGr should now work correctly with the Text tool. It will not trigger shortcuts
                            like File-&gt;Save All, or Edit-&gt;Paste into New Image. (thanks @Bruce Bowyer-Smyth for
                            the fix!)
                            <br>Changed: Image-&gt;Resize supports Super Sampling again, and favors this over Fant when
                            using Best Quality. Fant is still available, but is no longer chosen automatically.
                            <br>Changed: Holding Ctrl when starting to move a selection with the Move Selected Pixels
                            tool will no longer leave behind a copy of the selected area
                            <br>Fixed: Bicubic resampling in the Move Selected Pixels tool was not correctly handling
                            the alpha channel in some cases. This fix has required a reduction in performance.
                            <br>Improved: When using Edit-&gt;Copy, a 32-bit BGRA bitmap in the DIBV5 format is now
                            placed onto the clipboard so that other apps can read the alpha channel.
                            <br>Improved: When using Edit-&gt;Paste, DIBV5's are now supported if they have an alpha
                            channel. If they don't, then the regular DIB loader is used which has some heuristics for
                            detecting an incorrectly defined alpha channel and correcting for it.
                            <br>Improved: When using Edit-&gt;Paste, PNG is now the highest priority format. This
                            maximizes the ability to maintain alpha/transparency, but it does mean that images coming
                            from Microsoft Office apps will appear larger than they used to. This is either a bug or a
                            feature of Microsoft Office. For some reason it places PNGs on the clipboard that are 25%+
                            larger than the DIB/DIBV5 bitmap that it also places on the clipboard (but which don't have
                            alpha/transparency).
                            <br>Fixed: DIBV5 bitmaps should now work with Edit-&gt;Paste, which improves alpha channel
                            handling. (thanks @null54 for the fix!)
                            <br>Fixed: Top-down DIBs should now work correctly with Edit-&gt;Paste. (thanks @null54 for
                            the fix!)
                            <br>Improved CPU usage for thumbnail updates (layers and image tabs) in many cases.
                            <br>Improved: Slightly increased the size of the Settings dialog to reduce the need for
                            scrolling in a few important situations
                            <br>Fixed: Simple message boxes can now be closed with the ESC key
                            <br>Fixed: Magic Wand now works on very large images (e.g. 65535 x 65535 pixels) without an
                            error.
                            <br>New: Plugins that use IndirectUI can now use a UriProperty with a LinkLabel control
                            (thanks @null54!)
                            <br>New: Effect plugins can now more easily make use of the clipboard via the
                            IClipboardService. It will handle all of the tricky clipboard issues such as threading,
                            native data marshaling, and avoiding security vulnerabilities that exist in the standard
                            WinForms and WPF clipboard APIs.
                            <br>New: FileType plugins can now specify separate lists of extensions for loading and
                            saving.
                            <br>Blocked the WebP FileType v1.1.0.0 plugin due to instability. An update is already
                            available.
                            <br>Blocked the ImAgif FileType v0.12.0.1084 plugin due to incompatibility. An update will
                            hopefully soon be available.
                            <br>
                            <br>paint.net 4.1.6 - released on March 18th, 2019
                            <br>This update focuses on refreshing the app's theming with new high-res icons and improved
                            support for high-DPI configurations. Some new menu commands have been added, such as File
                            -&gt; Save All, and a Turkish translation has been added.
                            <br>New: Completely redone high-res icons throughout the app which match the Microsoft
                            Office style guidelines, with native support for up to 400% scaling (384 DPI)
                            <br>New: File -&gt; Save All (thanks @Bruce Bowyer-Smyth!)
                            <br>New: Turkish language
                            <br>New: Move Layer commands are now present in the Layers menu, not just on the Layers
                            window
                            <br>New: Layers -&gt; Rotate 180 (thanks @null54!)
                            <br>New: Plugins can now use the UIScaleFactor class, which simplifies making decisions
                            about DPI and scaling
                            <br>Improved: Image thumbnail list at the top of the main window now reacts to horizontal
                            mouse wheel or trackpad swiping
                            <br>Improved: The Text Tool's "Font Size Metric" button now has a tooltip explaining it
                            <br>Improved: When many images are open, Paint.NET now closes significantly faster (thanks
                            @Bruce Bowyer-Smyth for the fix!)
                            <br>Improved: File -&gt; Open Recent now has up to 10 images (up from 8 )
                            <br>Changed: Ctrl+Shift+F6 and +F7 will now also reset the floating window sizes for History
                            and Layers, respectively (same if you Ctrl+Shift+Click on the button at the top-right of the
                            main window)
                            <br>Changed: (for plugins) EffectFlags.SingleRenderCall is deprecated. Plugins should use
                            the new EffectRenderingSchedule.None option instead.
                            <br>Changed: Settings -&gt; Plugin Errors now shows up even if there are no plugin errors.
                            This ensures consistency, especially with the newly asynchronous nature of plugin loading
                            (otherwise there's no way to distinguish "no errors" from "not done loading plugins").
                            <br>Fixed: Items in the File -&gt; Open Recent menu will no longer get bigger or smaller
                            when moving between monitors with different DPIs
                            <br>Fixed: An icon handle was being leaked every time a dialog was opened (thanks @null54
                            for the fix!)
                            <br>Fixed a crash when running GPU effects (e.g. Black &amp; White) on very large, very tall
                            images
                            <br>Fixed: "Bad" plugins can no longer ruin the undo system by rendering outside of the
                            selection (thanks @BoltBait for helping out with this!)
                            <br>
                            <br>paint.net 4.1.5 - released on December 4th, 2018
                            <br>This update focuses on improving performance (sometimes significantly) and fixing
                            important bugs.
                            <br>Improved: Image -&gt; Rotate should now complete almost instantly (thanks @Bruce
                            Bowyer-Smyth!)
                            <br>Improved: Optimized a portion of the rendering engine for newer CPU instruction sets
                            (SSE2, SSSE3, AVX2). Depending on zoom level, CPU type, and other factors, rendering
                            throughput has been improved by 10-50%.
                            <br>Improved: Some performance optimizations for code that uses the indexers on the Surface
                            class, which should improve effect plugin performance (thanks @Bruce Bowyer-Smyth!)
                            <br>Fixed: Shortcut keys for the Adjustments menu weren't working until after you opened the
                            menu for the first time
                            <br>Fixed: Canvas checkerboard, used to indicate transparent regions of the image, now
                            scales with DPI
                            <br>Fixed some of the more rare cases of the SEHException/AccessViolationException crash
                            caused by Direct2D
                            <br>Fixed: A bug in IndirectUI was resulting in a crash when using @BoltBait's Level Horizon
                            plugin
                            <br>Fixed: Per-user fonts no longer cause a crash for the Store version
                            <br>New: The paintdotnet: protocol now works for the Classic version
                            <br>Fixed: The p﻿aintdotnet: ﻿protocol should now work properly with paths that have spaces
                            in them
                            <br>Fixed: Hardened security for loading Custom Shape plugins via XAML (thanks @Bruce
                            Bowyer-Smyth!)
                            <br>
                            <br>paint.net 4.1.4 - released on November 4th, 2018
                            <br>This is a small update that fixes some important bugs and substantially improves plugin
                            loading performance.
                            <br>Improved: Massive startup performance improvement when lots of effect plugins are
                            installed
                            <br>Fixed a crash that would happen when closing an image, exiting the app, or sometimes
                            just at random. This was happening due to a bug in Direct2D where ID2D1EffectContext does
                            not honor the multithreaded initialization flag from its ID2D1Factory, and was thus
                            corrupting its own internal data structures when released on the finalizer thread.
                            <br>Fixed: DirectX 9 GPUs can now utilize hardware acceleration again (in 4.1.3 they were
                            forced to use software rendering)
                            <br>Fixed: The Black &amp; White and Invert Colors adjustments no longer display an
                            OK/Cancel dialog
                            <br>
                            <br>paint.net 4.1.3 - released on October 24th, 2018
                            <br>This is a hotfix that addresses a crash which was affecting systems with pre-DirectX 10
                            GPUs.
                            <br>Fixed a crash when zooming due to missing pixel shader support on DX9 class GPUs
                            <br>
                            <br>paint.net 4.1.2 - released on October 22nd, 2018
                            <br>This is a small update that improves startup performance, fixes some bugs, and addresses
                            two security vulnerabilities. Administrators who manage deployments of Paint.NET are urged
                            to begin updating immediately. Details of CVE-2018-18446 and CVE-2018-18447 are pending
                            publication.
                            <br>Improved startup performance if "a lot" of effect plugins are installed. More
                            optimizations are coming in the next update.
                            <br>Fixed: Pixel grid no longer draws some dots darker than others at some zoom levels, as
                            reported at
                            https://forums.getpaint.net/topic/112794-pixel-grid-rendering-problems-when-zooming/
                            <br>Fixed: Radial Blur was not handling alpha correctly
                            <br>Fixed: IndirectUI ColorWheel swatch is now rendered correctly (without the fading alpha
                            gradient)
                            <br>Fixed: The tooltip describing the shortcut key for tools now indicates how many times to
                            press the key (e.g., press S four times for Magic Wand selection)
                            <br>Fixed: Pressing Escape to deselect now works with all tools (this bug was introduced in
                            v4.0)
                            <br>Fixed: Images with variable alpha were not displaying correctly at some zoom levels.
                            They were "too dark" in translucent regions. Reported here:
                            https://forums.getpaint.net/topic/112184-some-zoom-levels-display-alpha-as-extra-opaque/
                            <br>Fixed: For the Store release, launching with the paintdotnet: protocol no longer shows
                            an error if no parameters are provided (thanks @Bruce Bowyer-Smyth!)
                            <br>Fixed a crash for some effects that were rendering too quickly
                            <br>Fixed a bug in the Image&gt;Resize dialog where the asterisk and the note about which
                            resampling mode was being used, e.g. "* Bicubic will be used," weren't going away or
                            updating correctly
                            <br>New: Added a /set:SETTING=VALUE command-line parameter. This is specifically useful for
                            disabling hardware acceleration if the app won't start or you can't reach the Settings
                            dialog. This is also necessary for the Store release whose virtualized registry cannot be
                            edited. To launch the Store version with hardware acceleration disabled, go to Start -&gt;
                            Run and type in "paintdotnet:/set:UI/EnableHardwareAcceleration=false" (without quotes) and
                            press OK
                            <br>New: Added detection for when "Diebold Warsaw" is causing Paint.NET to crash. The error
                            message will indicate this cause.
                            <br>Fixed: Addressed CVE-2018-18446. Credit goes to Bruce Bowyer-Smyth.
                            <br>Fixed: Addressed CVE-2018-18447. Credit goes to Soroush Dalili from NCC Group.
                            <br>
                            <br>paint.net 4.1.1 - released on September 11th, 2018
                            <br>This is a hotfix that fixes a few small bugs, reinstates some keyboard shortcuts, and
                            adds 2 new languages.
                            <br>New: Ukranian translation
                            <br>New: Norwegian translation
                            <br>Fixed a bug in the IndirectUI color wheel control where it wouldn't pick up the correct
                            value for the alpha slider
                            <br>Fixed a crash with the new Shapes that would sometimes occur because the resources file
                            wasn't updated yet (probably due to a "you have to reboot" dialog at the end of updating
                            that was ignored)
                            <br>Reinstated the shortcut keys for the Adjustments menu, as this was a very unpopular
                            change
                            <br>Improved: IndirectUI angle chooser control now supports the UpDownIncrement property
                            (thanks @toe_head2001!)
                            <br>
                            <br>paint.net 4.1 - released on September 5th, 2018
                            <br>This update converts some effects to use the GPU for rendering, resulting in huge
                            performance gains. Copy/Paste can now be performed on selections, Bicubic resampling is now
                            available for the Move Selected Pixels tool, and there are lots of little quality-of-life
                            improvements and general bug fixes.
                            <br>Improved: Gaussian Blur, Motion Blur, and Radial Blur now render using the GPU and are
                            significantly faster
                            <br>Changed: The following effects are now rendered using the GPU: Edge Detect, Pixelate,
                            and Relief
                            <br>Changed: The following adjustments are now rendered using the GPU: Black &amp; White,
                            Invert Colors
                            <br>New Effect: Distort -&gt; Morphology (uses the GPU)
                            <br>New Effect: Render -&gt; Turbulence (uses the GPU)
                            <br>New: Bicubic resampling is now supported for the Move Selected Pixels tool. A CPU with 6
                            or more cores is highly recommended if you want to make it the default mode from within
                            Settings -&gt; Tools.
                            <br>New: Edit -&gt; Copy Selection. This will copy the current selection's geometry to the
                            clipboard as JSON text.
                            <br>New: Edit -&gt; Paste Selection. This will apply the selection from the clipboard to the
                            current selection. All 5 selection combine modes are supported.
                            <br>Changed: The Text tool now uses Points for font size measurement. You can also elect to
                            use the old font size metric, "Fixed (96 DPI)" via the dropdown to the right of the font
                            size.
                            <br>Fixed: The Text tool's recentering algorithm when typing reaches the edge of the
                            viewport should be better
                            <br>New: Added +/- buttons to the Tolerance and Hardness sliders.
                            <br>Changed: Increased max zoom level to 6400%
                            <br>New: The mouse wheel may now be used to scroll a long menu, such as when a lot of
                            effects are installed (thanks @toe_head2001!)
                            <br>Changed: For Windows 7 SP1 users, the Platform Update from 2013 is now required (it
                            contains Direct2D v1.1)
                            <br>Fixed: The "Finish" button wasn't working if it was in an overflow container (thanks
                            @toe_head2001!)
                            <br>Fixed: Opening certain large images and then zooming with the mouse wheel would
                            sometimes result in the scroll position being completely wrong
                            <br>Changed: Hiding a layer no longer auto-selects the nearest visible layer. You can
                            re-enable this in Settings, although this setting may be removed in a future version.
                            <br>New: For the Windows Store release, the paintdotnet: protocol can now be used to launch
                            the app so that you can specify command-line parameters. For example, you can go to Start
                            -&gt; Run and type in paintdotnet:"path to file1.png" path_to_file_2.png then both images
                            will be opened (even if Paint.NET is already open)
                            <br>New: Added Heptagon (7-sided polygon) and Octagon (8-sided polygon) shapes
                            <br>Fixed the high-DPI inset-text scaling for the Shape selector (e.g. Pentagon with an
                            inset "5")
                            <br>New: Palettes are now also loaded from Documents/paint.net App Files/Palettes. This
                            folder name is not localized so that installation scripts may easily make use of it
                            <br>Fixed: View -&gt; Pixel Grid will now correctly adjust to dynamic changes in the theme
                            (light vs. dark)
                            <br>Fixed: The background color for the Tolerance slider has been corrected for non-dark
                            themes
                            <br>Changed: Removed shortcut keys for all built-in Adjustments except for Invert Colors
                            (Ctrl+Shift+I). This is being done to free up shortcut keys for other functionality.
                            <br>New: Added a shortcut key to trigger a full .NET garbage collection: Ctrl+Alt+Shift+`
                            (tick/tilde). This should only ever be needed for troubleshooting purposes.
                            <br>New: Battery Saver Mode in Windows 10 is now respected, whether enabled manually or due
                            to low battery. UI animations will be disabled.
                            <br>New: Long file paths (&gt;MAX_PATH) are now supported on Windows 10, as long as the
                            group policy setting is enabled ("Enable Win32 long paths")
                            <br>New for plugin developers: The IndirectUI Color Wheel control now supports an alpha
                            slider. To use this, set the range (min/max values) of the Int32PropertyControl to
                            [Int32.MinValue, Int32.MaxValue] (thanks @BoltBait!)
                            <br>New for plugin developers: there is a new FileChooser property control type for string
                            properties (thanks @toe_head2001!)
                            <br>New for plugin developers: there is a new BinaryPixelOp.Apply(Surface, Surface, Surface,
                            Rectangle) method overload (thanks @BoltBait!)
                            <br>Changed: The IndirectUI text control now has a vertical scroll bar when multiline mode
                            is enabled (thanks @toe_head2001!)
                            <br>Changed: Visual C++ and OpenMP runtimes are now only loaded from the "app local" copy
                            (never from the system directory). This fixes a number of headaches, and also works around a
                            compatibility issue with the Surface Go
                            <br>Fixed: Crash when drag-and-dropping images onto Paint.NET when a tool was active but
                            with uncommitted changes
                            <br>Fixed a very old and nasty crash, "InvalidOperationException: ScratchSurface already
                            borrowed"
                            <br>
                            <br>paint.net 4.0.21 - released on January 14th, 2018
                            <br>This hotfix corrects a bug that was introduced when pasting images that are larger than
                            the canvas.
                            <br>Fixed a bug where a pasted image would be clipped after choosing "Keep canvas size"
                            <br>
                            <br>paint.net 4.0.20 - released on January 9th, 2018
                            <br>This update introduces a new Dark Theme, greatly improves High DPI support, adds
                            Explorer thumbnails for TGA and DDS image types, and fixes a lot of small bugs.
                            <br>New: Dark Theme support
                            <br>New: .NET Framework 4.7 is now required, and will be automatically installed if needed
                            <br>New: Explorer thumbnails are now supported for TGA and DDS file types
                            <br>Fixed and Improved: High-DPI support throughout the application
                            <br>Fixed: Color Picker tool was not always honoring the "Switch to previous tool" setting
                            <br>Fixed the arrow keys not working properly until the second shape (or line/curve) was
                            drawn. Reported here:
                            https://forums.getpaint.net/topic/112145-moving-points-in-lines-not-working-how-its-supposed-to/
                            <br>Fixed the zoom slider being "wiggly" while being dragged around
                            <br>Fixed a glitch with the mouse cursor (resize handle) at the lower-left corner of the
                            main window
                            <br>Fixed a crash in the Shape tool renderer (BadNumberException via
                            ID2D1Geometry::GetWidenedBounds)
                            <br>Fixed a hang in the Frosted Glass effect that was reported here:
                            https://forums.getpaint.net/topic/112005-frosted-glass-hangs-indefinitely-on-a-1x1-pixel-image/
                            <br>Fixed a hang in the Levels adjustment that was reported here:
                            https://forums.getpaint.net/topic/111629-hang-bug-in-a-levels-tool/
                            <br>Fixed a rendering issue in the Move Selected Pixels tool that was reported here:
                            https://forums.getpaint.net/topic/112187-selections-out-of-bounds-use-the-out-of-bounds-pixels-when-resizing/
                            <br>Fixed: Canvas now processes WM_MOUSEHWHEEL, which was preventing some horizontal mouse
                            wheels and trackpad swipe gestures from working properly
                            <br>Fixed: Plugins will no longer completely crash the app on Windows 10 S (note, however,
                            that plugins other than custom Shapes do not work on Windows 10 S)
                            <br>Fixed: a data loss bug when saving very large images (greater than 4GB). Reported here:
                            https://forums.getpaint.net/topic/111823-large-image-save-bug/
                            <br>
                            <br>paint.net 4.0.19 - released on October 2nd, 2017
                            <br>This is a hotfix that fixes a startup crash, and fixes Explorer thumbnails.
                            <br>Fixed missing thumbnails in Explorer for non-.PDN images (e.g. .PNG, .JPG), if Paint.NET
                            was configured to open these types by default
                            <br>Fixed a crash at startup that affected some people with a redirected Documents folder
                            (e.g. network share)
                            <br>
                            <br>paint.net 4.0.18 - released on September 29th, 2017
                            <br>This update improves performance and is the first version to be made available on the
                            Windows Store.
                            <br>Improved: Startup performance has been improved by about 25%
                            <br>New: Now available on the Windows Store!
                            https://www.microsoft.com/store/apps/9NBHCS1LX4R0
                            <br>Improved: Plugins can now be installed per-user into "Documents\paint.net App Files"
                            into folders named Effects, FileTypes, and Shapes. This is required for using plugins with
                            the Store release. To disable this (e.g. for administrators), set the
                            "Plugins/AllowLoadingPluginsFromUserLocations" key to "false" (HKLM\Software\paint.net).
                            <br>Improved: When using Portable Mode, custom palette files are stored next to the EXE
                            instead of in Documents
                            <br>Fixed: There was a crash on some systems that may have prevented the app from starting
                            up (MissingMethodException for "System.GC.Collect")
                            <br>
                            <br>paint.net 4.0.17 - released on July 20th, 2017
                            <br>This update improves performance and fixes a lot of small issues.
                            <br>Added: "Fluid mouse input" option in Settings -&gt; UI -&gt; Troubleshooting. If you see
                            major glitches while drawing, try disabling this.
                            <br>Improved: Default brush size, font size, and corner radius size now scales with major
                            DPI scaling levels (brush size of 2 at 100% scaling, brush size of 4 at 200% scaling, etc)
                            <br>Improved: Default image size now scales with major DPI scaling levels (800x600 at 100%,
                            1600x1200 at 200%, etc.)
                            <br>Improved performance and drawing latency by removing explicit calls to
                            System.GC.Collect() except when low memory conditions are encountered
                            <br>Improved performance by greatly reducing object allocation amplification by reducing the
                            concurrency level when using ConcurrentDictionary, and by removing WeakReference allocations
                            in favor of direct GCHandle usage
                            <br>Improved: Performance and battery usage by ensuring animations always run at the
                            monitor's actual refresh rate
                            <br>Improved (reduced) CPU usage when moving the mouse around the canvas
                            <br>Removed: "Hold Ctrl to hide handle" from the Text tool because it was not useful and
                            caused lots of confusion
                            <br>Fixed: Various high-DPI fixes, including horrible looking mouse cursors caused by a bug
                            in the latest .NET WinForms update
                            <br>Fixed: Gradient tool no longer applies dithering "outside" of the gradient (in areas
                            that should have a solid color)
                            <br>Fixed: Very slow performance opening the Effects menu when lots of plugins are installed
                            after installing the Windows 10 Creators Update
                            <br>Fixed: When cropping and then performing an undo, the scroll position was totally wrong
                            <br>Fixed a rendering glitch in the Save Configuration dialog (it would "wiggle")
                            <br>Fixed: At certain brush sizes, the brush indicator on the canvas had a visual glitch in
                            it due to a bug in Direct2D
                            <br>Fixed: Text tool buttons for Bold, Italics, Underline were not localized for a few
                            languages
                            <br>Fixed a rare crash in the taskbar thumbnails
                            <br>Fixed: Drawing with an aliased brush and opaque color (alpha=255) sometimes resulted in
                            non-opaque pixels due to a bug in Direct2D's ID2D1RenderTarget::FillOpacityMask
                            <br>Fixed: "Olden" effect should no longer cause crashes (it still has some rendering
                            artifacts due to its multithreading problems, however)
                            <br>
                            <br>paint.net 4.0.16 - released on April 16th, 2017
                            <br>This is a hotfix for a crash that results from copying images from some web browsers.
                            <br>Fixed a crash or hang that sometimes happens when copying images from Internet Explorer,
                            Edge, or Firefox, and then using File-&gt;New or Edit-&gt;Paste in paint.net.
                            <br>
                            <br>paint.net 4.0.15 - released on April 10th, 2017
                            <br>This is a hotfix that fixes a crash in the Magic Wand tool.
                            <br>Fixed a crash in the Magic Wand tool if it was used twice in a row with a selection mode
                            other than Replace.
                            <br>
                            <br>paint.net 4.0.14 - released on April 9th, 2017
                            <br>This is a minor update that slightly improves the brush tools, and fixes a few weird
                            issues that some people were seeing.
                            <br>Improved the performance of the Brush tools when antialiasing is enabled
                            <br>Improved the quality of the Brush tools when antialiasing is disabled
                            <br>Fixed: Edit-&gt;Paste wasn't working with some images that came from Firefox (as
                            discussed at
                            https://forums.getpaint.net/index.php?/topic/111012-not-enough-memory-to-paste-from-clipboard/
                            )
                            <br>Fixed: Improved the reliability of Image-&gt;Crop to Selection on 32-bit systems.
                            Instead of crashing when it runs out of memory, it will just show an error.
                            <br>Fixed: Reduced crashes when loading UI images caused by an unreliable Windows component
                            ("System.ArgumentException: Parameter is not valid")
                            <br>Fixed: When manually checking for updates in the Settings dialog and the user didn't
                            actually have the necessary security privileges, a crash might result instead of an error
                            dialog.
                            <br>
                            <br>paint.net 4.0.13 - released on December 12th, 2016
                            <br>This is a minor update that fixes a few high priority problems that many people were
                            bumping into.
                            <br>Fixed "Missing api-ms-win-core-timezone-l1-1-0.dll" error that was being seen on some
                            Windows 7 systems due to partial install or uninstall of Microsoft's Universal C Runtime
                            <br>Fixed the layout for the File-&gt;New, Image-&gt;Resize, and Image-&gt;Canvas Size
                            dialogs in all known situations (various languages, DPI sizes, font configurations)
                            <br>Fixed: Old versions of PSD plugin couldn't load due to removal of PrivateThreadPool
                            <br>Fixed a crash when typing a negative number for a zoom level
                            <br>
                            <br>paint.net 4.0.12 - released on September 12th, 2016
                            <br>This is a hotfix that fixes some crashing on single CPU systems, and a rendering bug in
                            the Rounded Rectangle shape.
                            <br>Fixed: The Rounded Rectangle shape's rendering was incorrect for some values of "Corner
                            size"
                            <br>Fixed: Effects and Adjustments were crashing the app on systems with only 1 CPU core, or
                            virtual machines configured for only 1 CPU
                            <br>
                            <br>paint.net 4.0.11 - released on September 10th, 2016
                            <br>This update adds the ability to configure the Rounded Rectangle shape's corner size. It
                            also fixes issues with scrolling and panning, effect rendering performance, high DPI, and a
                            rare system hang caused by WPF.
                            <br>New: The Rounded Rectangle shape's corner size ("radius") is now configurable
                            <br>New: Overscroll can now be disabled from within Settings
                            <br>Fixed: The Zoom tool was broken in 4.0.10
                            <br>Fixed: Auto scroll will no longer engage overscroll. This prevents the image from
                            shooting off in all directions when drawing on it or when making a selection.
                            <br>Fixed: Panning with the middle mouse button would sometimes be "sticky", as reported at
                            http://forums.getpaint.net/index.php?/topic/110131-dragging-with-the-mouse-wheel-is-sticky/
                            <br>Fixed: Effect rendering performance had significantly regressed in 4.0.10, by as much as
                            50%, on Intel CPUs with HyperThreading.
                            http://forums.getpaint.net/index.php?/topic/110090-paintnet-run-significantly-slower-on-windows-10-compared-to-windows-7/
                            <br>Fixed: Selecting the entire image and then using Zoom to Selection or the Zoom Tool
                            would align the image in an awkward manner
                            <br>Fixed: In rare cases, Settings -&gt; Plugin Errors was hanging the whole system (bug in
                            WPF?). This UI is now implemented in WinForms instead of WPF.
                            http://forums.getpaint.net/index.php?/topic/110002-plugin-error-screen-complete-pc-freezelockout/
                            <br>Fixed: Some more high-DPI issues, especially when using multiple monitors with mixed
                            DPI, or when using Remote Desktop
                            <br>
                            <br>paint.net 4.0.10 - released on July 8th, 2016
                            <br>This update introduces overscroll, the ability to scroll the canvas past the image
                            boundaries. It also includes a big serving of other minor fixes.
                            <br>New: The canvas may now be scrolled past the edge of the image
                            <br>New: When holding the spacebar, you may scroll using the keyboard arrow keys (in
                            addition to click-and-drag panning). Holding Ctrl will scroll at 10x the rate.
                            <br>New: You can now hold Ctrl+Shift while clicking on the floating window icons in order to
                            reset their location and docking. Ctrl+Shift along with the appropriate hotkey (F5, F6, F7,
                            F8) also does the trick.
                            <br>Improved: The rate of auto-scrolling, which triggers when the mouse is at the canvas
                            edge and a button is being held down, has been improved and is based on time instead of
                            frames
                            <br>Improved: Fixed Size selection drawing now defaults to 400x300 pixels instead of 4x3
                            inches
                            <br>Improved: Tooltips for Custom Shapes now include their file system location
                            <br>Improved: Edit-&gt;Invert Selection should perform much faster when used with unmodified
                            selections from the Magic Wand tool
                            <br>Improved: When running within VMWare, "Hardware accelerated rendering" is disabled by
                            default (Microsoft's WARP is faster than VMWare's D3D emulation)
                            <br>Fixed: Erratic brush/pencil drawing when running within VMWare (this is caused by a bug
                            in Win32's GetMouseMovePointEx API, and is not actually limited to VMWare)
                            <br>Fixed: Color Picker tool could crash if used at the bottom of the image, as reported at
                            http://forums.getpaint.net/index.php?/topic/109248-paintnet-crashes-when-color-picker-off-screen-update/
                            <br>Fixed: There was a glitch in the Gradient tool's rendering when dx was equal to dy, as
                            reported at
                            http://forums.getpaint.net/index.php?/topic/107380-gradient-bugs-in-direction-and-length/
                            <br>Fixed: The Layers window would sometimes auto-scroll the active layer to the bottom when
                            performing certain operations, as reported at
                            http://forums.getpaint.net/index.php?/topic/32527-layers-auto-scrolling-when-adding-or-duplicating/
                            <br>Fixed some mouse cursor glitches when using panning using the spacebar
                            <br>Fixed many glitches and a few crashes in the image size dialogs (File-&gt;New,
                            Image-&gt;Resize, Image-&gt;Canvas Size)
                            <br>Fixed a problem with inconsinstently skipped input when using the arrow keys to move
                            tool handles, as reported at
                            http://forums.getpaint.net/index.php?/topic/108932-selected-area-moving-with-direction-keys-bug/
                            <br>Fixed: Custom Shapes did not always have the correct bounding box, and would have weird
                            behavior as a result
                            <br>Fixed: Line/Curve handles were unusable for up to 500ms after adjusting properties in
                            the toolbar
                            <br>Fixed some crashes and soft hangs in the Save Configuration dialog
                            <br>Fixed a blemish at the top of the main window when Windows is set to 200% DPI
                            <br>Fixed: There were some precision bugs with IndirectUI sliders that would cause them to
                            get "stuck" at certain values (mostly affects effect plugins)
                            <br>Improved: IndirectUI's Angle Chooser control now supports the DecimalPlaces property
                            (for plugins)
                            <br>Improved: IndirectUI's Slider controls now support all-negative ranges (e.g. [-200,
                            -20])
                            <br>
                            <br>paint.net 4.0.9 - released on January 5th, 2016
                            <br>This is an update that fixes a few crashes and bugs that were found in 4.0.8.
                            <br>Fixed: Selection tools would sometimes crash
                            <br>Fixed: Line/Curve tool would draw nothing if the Shapes tool was configured for "Draw
                            Filled Shape"
                            <br>Fixed: Thumbnails for .PDN files were not working on some systems
                            <br>Fixed: The "Finish" button in the toolbar would not update its enable/disable state when
                            switching between images
                            <br>
                            <br>paint.net 4.0.8 - released on December 30th, 2015
                            <br>This is a hotfix that fixes a crashing bug with the Line/Curve tool in 4.0.7.
                            <br>Fixed: The Line/Curve tool was crashing when drawing vertical lines of particular
                            lengths.
                            <br>
                            <br>paint.net 4.0.7 - released on December 30th, 2015
                            <br>This update improves performance in several key areas, fixes accent color support in
                            Windows 10, and fixes many important bugs and crashes.
                            <br>Changed: .NET Framework 4.6 is now required, and will be installed if necessary
                            <br>New: Swedish translation
                            <br>Fixed: Title bar now uses the Windows 10 accent color
                            <br>Fixed: Floating windows were not remembering their locations on some non-English systems
                            <br>Improved: Performance of "committing" (finishing) is now up to 10x faster, which greatly
                            improves responsivness for quick drawing operations
                            <br>Improved Shapes tool quality when drawn without antialiasing, with line styles, and at 1
                            pixel brush width
                            <br>Improved Shapes tool rendering performance on CPUs with many cores (8+)
                            <br>Improved: Installing a "complex" custom Shape no longer causes very long hangs at app
                            startup
                            <br>Improved: Image-&gt;Resize is now much faster
                            <br>Fixed: Image-&gt;Resize would sometimes cause the main window to flicker or lose focus
                            <br>Fixed: Image-&gt;Resize would sometimes do nothing instead of resizing the image to a
                            very large size
                            <br>Fixed: Labels on the vertical ruler were misleading because they were on the wrong side
                            of the tick mark
                            <br>Improved the ruler's performance
                            <br>Fixed: Edit-&gt;Copy now works if the data copied to the clipboard is larger than 2GB
                            <br>Fixed: Page Up, Page Down, Home, and End keys now work in the main canvas area
                            <br>Fixed: Paint.NET will no longer incorrectly block Windows from restarting
                            <br>Fixed: Rotate/Zoom no longer crashes on very large images
                            <br>Improved: Reduced CPU/GPU and battery use when the app is not in the foreground
                            <br>Improved: Reduced CPU and battery use of the UI for the Move and Shapes tools
                            <br>Added: Custom Shapes XAML now supports cardinal splines via PolyCurveSegment (a new
                            PathSegment type)
                            <br>Improved: Various performance improvements
                            <br>Fixed: Several rare or uncommon crashes
                            <br>
                            <br>paint.net 4.0.6 - released on August 2nd, 2015
                            <br>This update adds the ability to install custom shapes, is updated for Windows 10, and
                            fixes some minor bugs and crashes.
                            <br>New: You can now create and install custom shapes for the Shapes tool.
                            <br>New: Updated to work better with Windows 10.
                            <br>New: Increased the maximum brush size to 2000.
                            <br>New: IndirectUI-based effect plugins can now provide help text, accessible via the
                            question mark button.
                            <br>New: Effect plugins may now access the current palette via IPalettesService.
                            <br>Improved: Reduced memory usage of brush tools when using large brush sizes.
                            <br>Fixed: Holding shift to constrain the angle of the roll control (Layers -&gt;
                            Rotate/Zoom) wasn't working correctly.
                            <br>Fixed: Various shapes (hexagon, pentagon, triangle, etc.) are now symmetric when holding
                            the shift key.
                            <br>Fixed: Multiple high-dpi blemishes in the main window and many dialog boxes (Settings,
                            Save Configuration, all effect dialogs, etc.)
                            <br>Fixed: Various minor/rare crashes.
                            <br>
                            <br>paint.net 4.0.5 - released on December 7th, 2014
                            <br>This update fixes a few important bugs, some of which were introduced in 4.0.4.
                            <br>Fixed: Subtraction mode in the Magic Wand tool was generating B-A instead of A-B.
                            <br>Fixed: Crash when using Effect-&gt;Repeat.
                            <br>Fixed: Crash (AccessViolationException) on some systems when initializing the canvas for
                            hardware accelerated rendering. It will still crash but then switch to software rendering
                            for the next startup, which will then avoid the crashing.
                            <br>Fixed: Crash when clicking on the Shapes tool if you had run an old 4.0 beta/alpha and
                            had also changed which shape is used at startup to be a line or curve.
                            <br>Fixed: Crash when using Settings -&gt; Update -&gt; Check Now due to incorrectly
                            determining that UAC is not enabled.
                            <br>
                            <br>paint.net 4.0.4 - released on November 29th, 2014
                            <br>This update greatly improves performance in some key areas, fixes some important bugs,
                            and reintroduces a feature that was omitted in the transition from 3.5 to 4.0.
                            <br>New: Added a 'Fill' property to the Paintbrush tool (regression from 3.5).
                            <br>Faster: Move Selected Pixels has been significantly optimized.
                            <br>Faster: Magic Wand Tool has been significantly optimized.
                            <br>Faster: Working with aliased selections ("aliased selection quality" in the toolbar) has
                            been significantly optimized.
                            <br>Faster: Edit-&gt;Copy and Edit-&gt;Copy Merged are now up to 2x faster.
                            <br>Faster: Drawing when a selection is active; clipping performance is now improved.
                            <br>Fixed: The Text tool no longer produces terrible looking text when using Smooth
                            rendering mode without antialiasing.
                            <br>Fixed: The Gear shape had a few glitches.
                            <br>Fixed: Using a Fill pattern with the Paint Bucket would sometimes produces misaligned or
                            "corrupt looking" results.
                            <br>Fixed: The alignment of the menu buttons in the top-right was off by 2 pixels, causing
                            them to look weird at high-DPI.
                            <br>Fixed: The zoom buttons in the status bar would not recognize clicks unless the main
                            window was already in focus.
                            <br>Fixed: Some incorrect errors about requiring Windows 7 SP1 when launching the installer
                            from something like an old version of WinZip.
                            <br>Fixed: Edit-&gt;Clear Selection and Edit-&gt;Cut were filling with transparent black
                            (#00000000) instead of transparent white (#00FFFFFF). This caused some discrepancies
                            compared to older versions of Paint.NET (regression from 3.5).
                            <br>Fixed: Pressing Ctrl+A when a drawing tool was active would sometimes incorrectly show a
                            tinted selection.
                            <br>Fixed: Text in the title bar was not visible when using a 3rd party Aero theme with
                            black titlebars.
                            <br>
                            <br>paint.net 4.0.3 - released on July 22nd, 2014
                            <br>This update fixes a few small bugs and improves performance.
                            <br>Further improved performance when working with images that have a lot of layers.
                            <br>Fixed some flickering in the Layers form.
                            <br>Fixed the Language selector in the Settings dialog.
                            <br>Fixed 2-finger touchpad and touch screen scrolling.
                            <br>Aero peek thumbnails now include the pixel grid if it's enabled.
                            <br>Fixed a crash in the thumbnail renderer that sometimes happened when switching between
                            images.
                            <br>Ctrl+W no longer exits the application if zero images are open.
                            <br>
                            <br>paint.net 4.0.2 - released on July 15th, 2014
                            <br>This update fixes a few small bugs and feature regressions from 3.5.
                            <br>Fixed the gamma and contrast for text rendering on some systems where the wrong values
                            were being used ("rainbow" text)
                            <br>Colors window now correctly lets you paste a hex color value that starts with a hash,
                            e.g. #112233
                            <br>Gradient tool now lets you reverse a transparency gradient by clicking the right mouse
                            button on one of the handles (regression from 3.5)
                            <br>Move Selected Pixels now lets you hold Control to leave a copy of the selected area
                            behind on the initial move (regression from 3.5)
                            <br>Paint Bucket tool's hatch fill modes weren't working with the Overwrite blending mode
                            (regression from 3.5)
                            <br>Fixed a keyboard tabbing issue in the Resize dialog (regression from 3.5)
                            <br>Fixed the language setting in the Settings dialog not always allowing you to set it to
                            English if your system's default language is non-English
                            <br>Fixed a performance issue that caused images with many layers (50+) to take a VERY long
                            time to open, close, or even switch away from (regression from 3.5)
                            <br>Fixed a rare crash at application exit
                            <br>Fixed an issue that prevented 4.0.1 from installing on top of 4.0 when using the MSI
                            (e.g. AD/GPO network deployment)
                            <br>Fixed an issue that would sometimes cause the installer to take 30+ seconds to appear
                            <br>
                            <br>paint.net 4.0.1 - released on July 12th, 2014
                            <br>This update is focused on fixing some important crashes, bricks, and functionality
                            issues, and also on a few key performance optimizations.
                            <br>Move Selected Pixels tool performance has been significantly optimized.
                            <br>Move Selected Pixels tool was always leaving transparent black behind instead of the
                            secondary color with alpha removed.
                            <br>Brush tools with odd-sized brushes and no antialiasing were drawing at 1 size smaller.
                            <br>Fixed some apparent ‘lag’ in the brush tools due to an off-by-1 glitch in the stroke
                            path calculation code.
                            <br>The brush tool preview circle no longer scales by the system DPI setting, which made it
                            too big.
                            <br>Removed the momentary hourglass/wait cursor after drawing (e.g. pencil and brush tools).
                            <br>Optimized performance of the Shapes tool, especially for the Ellipse shape.
                            <br>Paint Bucket tool will now correctly treat the selection as a boundary contour.
                            <br>Zoom tool no longer crashes sometimes when pressing the right mouse button while already
                            holding the left mouse button.
                            <br>The status bar now reports the correct selection location when it’s outside the image
                            boundaries (e.g. negative values).
                            <br>Auto-scrolling on the edge of the window now works correctly and doesn’t require you to
                            "jiggle the mouse" for each scroll update.
                            <br>Touch screens no longer scroll when swiping up/down with one finger.
                            <br>Improved the pixel grid’s contrast so it’s not overwhelmingly bright.
                            <br>The transparency "checkerboard" is now aligned to the top-left of the image, instead of
                            the top-left of the canvas.
                            <br>The cursor position reported in the status bar was off-by-1 when the value was supposed
                            to be negative.
                            <br>Some controls (e.g. units selection in the Image-&gt;Resize dialog) were not drawing
                            focus rectangles when using the keyboard.
                            <br>Fixed a crash (OutOfMemoryException) when using a selection tool when hardware
                            acceleration is disabled.
                            <br>Fixed a crash (TimeBeforeLastUpdateException) in the installer. This usually happens
                            when running in a virtual machine, and only affects animations.
                            <br>Fixed a crash (BadImageFormatException) at startup. This indicates an installation
                            error, and will be automatically repaired.
                            <br>Fixed various crashes caused by having the wrong (old) version of
                            PaintDotNet.SystemLayer.Native.dll. This indicates an installation error, and will be
                            automatically repaired.
                            <br>Improved performance when software rendering is used (e.g. when hardware accelerated
                            rendering is disabled).
                            <br>All 7th generation Intel GPUs now default to hardware rendering. All older Intel GPUs
                            default to software rendering.
                            <br>Fixed graphical artifacts (blackness, flickering, mouse trails) on certain GPUs (e.g.
                            NVIDIA Optimus).
                            <br>NVIDIA ION graphics cards now default to software rendering due to crashes.
                            <br>Fixed an issue that was causing beta updates to be offered even if “Also check for
                            pre-release (beta) versions of paint.net” was disabled in Settings
                            <br>paint.net 4.0 - released on June 24th, 2014
                            <br>This release improves performance and memory usage with a new rendering engine optimized
                            for multicore CPUs and hardware acceleration (GPU). Most tools now support "fine grained
                            history" and live adjustment of their properties, including the Magic Wand and Paint Bucket.
                            Selections are now antialiased, which greatly improves their quality.
                            <br>
                            <br>System Requirements
                            <br>Windows 7 SP1 or newer is now required.
                            <br>.NET Framework 4.5 is now required, and will be installed if needed.
                            <br>A dual-core (or more!) processor is highly recommended.
                            <br>Hardware acceleration (GPU) via Direct2D is now supported.
                            <br>Please disable this in the Settings dialog if you experience visual artifacts.
                            <br>Performance
                            <br>A brand new, asynchronous, fully multithreaded rendering engine allows performance to
                            scale very well with respect to the number of CPU cores whether you have 2, 4, 6, or even 16
                            of them.
                            <br>The responsiveness of the user interface has been greatly improved, especially when
                            working with large images.
                            <br>Memory usage is lower.
                            <br>Improved battery life impact due to fixing the way the floating windows manage their
                            transparency.
                            <br>Startup performance when many plugins are installed is improved, thanks to the Multicore
                            JIT feature introduced in .NET 4.5.
                            <br>Selections
                            <br>Selections are now antialiased, which greatly improves the quality around the edges of
                            selected content. You can turn this on and off at any time from the toolbar.
                            <br>Everything related to selections now has much higher performance and greatly reduced CPU
                            usage, especially if hardware acceleration (GPU) is enabled.
                            <br>The selection outline is now rendered using the "dancing ants" animation, which greatly
                            improves the contrast between it and the image itself.
                            <br>General
                            <br>The functionality previously provided by the Utilities, Window, and Help menus has been
                            simplified, consolidated, and moved to the top-right corner of the main window.
                            <br>
                            <br>The image thumbnail list has been moved up 1 row so that it no longer intrudes into the
                            current Tool's toolbar space. This means it will no longer "jump around" when you switch
                            between tools. This also means that it is aligned to the top of the monitor when the main
                            window is maximized, making it easier to click on images (Fitt's law).
                            <br>The image thumbnail list can now be reordered with drag-and-drop.
                            <br>A brand new Settings dialog makes it much easier to configure all the tool and toolbar
                            defaults, among other things.
                            <br>The zoom slider and units selector have been moved from the toolbar to the bottom right
                            corner of the window (into the status bar).
                            <br>Each image now shows up as its own taskbar item. This can be disabled in the Settings
                            dialog with "Show image previews in the Windows taskbar."
                            <br>Layers can now be reordered with drag-and-drop.
                            <br>Ctrl+Click on the Move Layer Up/Down buttons will now move a layer to the top/bottom,
                            respectively.
                            <br>Improved quality of Image -&gt; Resize.
                            <br>Edit -&gt; Copy Merged will copy all layers to the clipboard without having to use Image
                            -&gt; Flatten first.
                            <br>Copying to the clipboard now includes the "PNG" format, which allows transparency to
                            survive from many popular applications (e.g. Office)
                            <br>You can now use the middle mouse button to scroll/pan the image at any time (same
                            functionality as holding down the spacebar along with clicking and dragging the mouse).
                            <br>Shift+Backspace will now fill the selection with the secondary color (Backspace, the
                            shortcut key for Edit -&gt; Fill Selection, still fills with primary color as usual).
                            <br>paint.net now shows up in Windows' “Default Programs” control panel so you can configure
                            its file type associations without reinstalling.
                            <br>EXIF rotation metadata is now applied when opening images (e.g. JPG taken with a rotated
                            camera).
                            <br>Eleven (11) new languages, bringing the total to 21: Chinese (Simplified), Chinese
                            (Traditional), Czech, Danish, Dutch, English, Finnish, French, German, Hindi, Hungarian,
                            Italian, Japanese, Korean, Lithuanian, Persian, Polish, Portuguese (Brazilian), Portuguese
                            (Portugal), Russian, and Spanish.
                            <br>Crash logs are now stored in %LOCALAPPDATA%\paint.net\CrashLogs (e.g.
                            C:\Users\username\AppData\Local\paint.net\CrashLogs) instead of on the desktop.
                            <br>Effects
                            <br>New effect: Photo -&gt; Vignette.
                            <br>Improved the quality of the Photo -&gt; Red Eye Removal effect.
                            <br>Improved UI for Layers -&gt; Rotate/Zoom.
                            <br>Effect plugins now show up with a jigsaw puzzle icon next to them in the menus. You can
                            hover over the effect to see information about it, including the author and location of its
                            DLL.
                            <br>Errors while loading effect plugins are now displayed in the Settings dialog.
                            <br>Tools
                            <br>Most Tools now support "fine-grained history." You may adjust the properties of what
                            you've drawn (e.g. colors, toolbar settings) before committing to the layer (use the
                            "Finish" button or press Enter), and each change is tracked in the history.
                            <br>Tools may now draw directly with a blending mode, configurable from the toolbar. All of
                            the layer blending modes are supported, as well as “Overwrite.”
                            <br>
                            <br>Drawing tools (Pencil, Paintbrush, Eraser, Clone Stamp, Recolor) now have much smoother
                            mouse input handling via GetMouseMovePointsEx.
                            <br>Brush tools (Paintbrush, Eraser, Clone Stamp, Recolor) now have soft brushes support via
                            a “Hardness” setting in the toolbar.
                            <br>The Move tools (Move Selected Pixels, Move Selection) have a much better UI for scaling,
                            moving, and (especially) rotation.
                            <br>The Move tools now support moving the rotation anchor, which changes the center of
                            rotation.
                            <br>The new Shapes tool replaces the Rectangle, Rounded Rectangle, Ellipse, and Freeform
                            shape tools. 27 shapes are currently available. You may move, resize, and rotate a shape, as
                            well as reconfigure any other properties from the toolbar (color, outline size, etc.) before
                            committing it to the layer.
                            <br>Color Picker has a configurable sampling radius, and can sample from either the current
                            layer or the whole image.
                            <br>Gradient tool now supports a new Spiral gradient type and allows configuration of the
                            repeat mode (none, repeat, wrapped).
                            <br>Gradient tool has improved rendering quality via dithering and antialiasing. You can
                            control both of these with the standard antialiasing toggle in the toolbar.
                            <br>Magic Wand and Paint Bucket now allow live adjustment of Tolerance and the Origin (click
                            location) after clicking (press Enter to commit/finish).
                            <br>Magic Wand and Paint Bucket can now sample from either the current layer or the whole
                            image.
                            <br>Paint Bucket tool now supports anti-aliasing.
                            <br>Recolor tool can now use the color of the pixel where you click as the color to be
                            replaced. Or, as usual, it can use the secondary color.
                            <br>Text tool now supports multiple rendering modes: Smooth, Sharp (Modern), and Sharp
                            (Classic). These correspond to DirectWrite rendering modes of Outline, ClearType Natural
                            Symmetric, and GDI Classic, respectively.
                            <br>Text tool now supports colored fonts on Windows 8.1.
                            <br>Paint.NET v3.5.11 - released on August 17th, 2013
                            <br>The primary goal of this update is preparing for the v4.0 release: previous versions of
                            Paint.NET will not be able to offer the v4.0 update. Also included are some small fixes and
                            performance improvements that have been ported over from the v4.0 codebase.
                            <br>
                            <br>Fixed: The Gaussian Blur effect was incorrectly calculating alpha values for non-opaque
                            pixels.
                            <br>Improved performance of the Sharpen effect by about 25%
                            <br>Improved performance of the Median effect by about 30%
                            <br>Improved performance of the Fragment effect by about 40%
                            <br>Improved performance of the Unfocus effect by about 100%
                            <br>Reduced memory usage when many selection manipulation operations are in the history/undo
                            stack (the undo data is now saved to disk)
                            <br>The built-in updater now supports upgrading to paint.net 4.0 (when it's available)
                            <br>Paint.NET v3.5.10 - released on October 9th, 2011
                            <br>This update fixes some broken shortcut keys for the View -&gt; Actual Size command.
                            <br>
                            <br>Fixed: Ctrl+Shift+A now works again as a shortcut for View -&gt; Actual Size (broken in
                            3.5.9)
                            <br>Fixed: Ctrl+0 still works for View -&gt; Actual Size even if 10 or more images are open
                            (broken in 3.5.9, it would switch to the 10th image).
                            <br>Paint.NET v3.5.9 - released on October 1st, 2011
                            <br>This update improves the "Auto-Detect" bit-depth feature, and fixes a few small issues.
                            <br>
                            <br>Improved: The "Auto-detect" bit-depth setting for PNG, BMP, and TGA now also determines
                            which bit-depth to use based on which one produces the smallest file size, as well as which
                            ones can save the image without losing fidelity.
                            <br>Improved: You can now use Ctrl+0 as a shortcut key for View -&gt; Actual Size, in
                            addition to Ctrl+Shift+A and Ctrl+Alt+0.
                            <br>Fixed: Some text in the DirectDraw Surface (DDS) Save Configuration UI was not being
                            loaded.
                            <br>Fixed: Some DirectDraw Surface (DDS) files authored with other software (e.g. Unreal
                            2004) could not be loaded.
                            <br>Fixed: In some rare circumstances, clicking on the Save button in the toolbar would
                            crash.
                            <br>Fixed: The Korean translation has been added back in, with the help of Bing machine
                            translation to cover the few remaining strings that were untranslated.
                            <br>Paint.NET v3.5.8 - released on March 5th, 2011
                            <br>This update fixes some issues with the fault-tolerant save feature introduced in 3.5.7.
                            <br>
                            <br>Fixed: Saving to a folder that has been moved or renamed will display an error instead
                            of crashing (regression from 3.5.6)
                            <br>Fixed: Saving to a Sharepoint site will now work (regression from 3.5.6)
                            <br>Fixed: Saving to a file that is marked as read only will now give an error instead of
                            crashing (regression from 3.5.6)
                            <br>Fixed: General reliability and correctness improvements to fault-tolerant saving
                            <br>Paint.NET v3.5.7 - released on February 20th, 2011
                            <br>This update improves reliability of saving, further improves Copy/Paste functionality,
                            and fixes some other miscellaneous bugs.
                            <br>
                            <br>Saving an image is now fault-tolerant. If there is an error or crash while saving, the
                            original file will be left alone.
                            <br>Worked around a bug in some plugins that are incorrectly using the built-in Gaussian
                            Blur effect. For example, Sharpen+. Now they won't crash.
                            <br>Fixed a bug with Edit-&gt;Paste into New Image, where the new image would be 1 pixel too
                            wide or tall, as reported at
                            http://forums.getpaint.net/index.php?/topic/20969-paste-problem/
                            <br>Fixed a bug with the Rectangle Select tool and Fixed Ratio selection, which would be off
                            by 1 pixel, as reported at
                            http://forums.getpaint.net/index.php?/topic/20820-croppig-by-fixed-ratio-is-inexact
                            <br>When pasting an image from Paint.NET into Paint.NET, it will be a little smarter about
                            where it puts the image. Previously, if the location wasn't within the viewport, it would be
                            placed at the top-left corner of the viewport. Now it will find the nearest point along the
                            edge of the viewport to place the image.
                            <br>The EXIF rotation ("orientation") metadata is now discarded when opening an image, which
                            was causing aggravation with images that could then never be reoriented correctly using
                            Image-&gt;Rotate
                            <br>The EXIF metadata for JPEG thumbnail data are now correctly discarded.
                            <br>Fixed a handful of memory leaks.
                            <br>Fixed a typo in the Italian translation. In the setup wizard it was referring to
                            "Pain.NET" (woops)
                            <br>Paint.NET v3.5.6 - released on November 18th, 2010
                            <br>This update fixes several issues related to copy-paste, improves performance and quality
                            for a few adjustments, and fixes a data loss bug.
                            <br>
                            <br>When pasting an image, Paint.NET will be smarter about ensuring it is placed within the
                            area that has been scrolled/zoomed to.
                            <br>Improved the performance and quality of the Curves and Hue/Saturation adjustments.
                            <br>Some minor improvements to memory usage, which should help out a few scenarios on 32-bit
                            systems.
                            <br>Fixed: If a JPEG was loaded that had an embedded ICC profile, and was then saved as an
                            8-bit or 24-bit PNG, then the resulting file would be corrupt (32-bit PNG worked fine
                            though).
                            <br>Fixed: 16-bit TGAs no longer load with the red and blue channels swapped.
                            <br>Fixed: Copy-paste from a Remote Desktop session will no longer be 'shifted' by 3 pixels.
                            <br>Fixed: Copy-paste from Internet Explorer, Firefox, or Chrome should preserve
                            alpha/transparency.
                            <br>Fixed: Copying from Paint.NET and pasting into Windows Live Writer should now work.
                            <br>Fixed: Taking a full-screen screenshot with Print Screen on a multimonitor system, where
                            those monitors don't form a simple rectangle, will now fill the 'gap area' with transparent
                            instead of black. (Example: two monitors of the same size, one of which is rotated by 90
                            degrees)
                            <br>Fixed: If Paint.NET is opened without specifying an image to open, and then the default
                            image is modified and saved, then Paint.NET will no longer close it upon opening another
                            one. This was causing data loss if that default image had layers, and was then saved in a
                            format that did not support layers (anything other than .PDN).
                            <br>Fixed: Some systems were showing 'red X' thumbnails for .PDN files in Windows Explorer,
                            instead of the real thumbnail.
                            <br>Fixed: The EXIF "Creation Software" saved along with images is no longer localized. This
                            prevents certain languages from seeing "Paint.NET ????? v3.5.6" in the image properties
                            (metadata).
                            <br>Paint.NET v3.5.5 - released on April 25th, 2010
                            <br>This update fixes a bug when saving 8-bit images, improves layer composition and
                            Gaussian Blur performance, and is now updated to support the new .NET Framework 4.0 in some
                            cases.
                            <br>
                            <br>Fixed the bug where saving as 8-bit PNG/GIF/BMP wasn't always working, usually with
                            larger images.
                            <br>Improved the performance of the Gaussian Blur effect by 30-40%.
                            <br>Improved the performance of all the layer blending modes by 15-30%.
                            <br>Improved the performance of zooming with the mouse wheel on dual-core Intel Atom
                            systems.
                            <br>Updated to support .NET 4.0 if no other version of .NET is installed.
                            <br>Reduced download size from 4.8MB down to 3.5MB.
                            <br>Fixed a small error in the Chinese translation.
                            <br>Please note that the system requirements have been updated. For Windows XP, you must now
                            have Service Pack 3 (SP3) installed; SP2 is no longer supported. For Windows Vista, you must
                            now have Service Pack 1 installed.
                            <br>
                            <br>Paint.NET v3.5.4 - released on February 25th, 2010
                            <br>This update fixes a few small bugs, and improves performance of the Flatten command.
                            <br>
                            <br>Improved performance of the Image-&gt;Flatten command by making it multithreaded.
                            <br>Fixed the File-&gt;Save As dialog not opening to the correct folder.
                            <br>Fixed a crash with certain plugins and their use of the File Open dialog.
                            <br>Fixed a very rare crash with the toolbar's font list.
                            <br>Paint.NET v3.5.3, released on February 7th, 2010
                            <br>This update fixes a few small bugs.
                            <br>
                            <br>Fixed DirectDraw Surface (.dds) file format support for CPUs which do not have SSE2
                            (Pentium III, Athlon XP).
                            <br>Fixed an issue with the File-&gt;Save dialog related to file type plugins that were only
                            written for opening (importing).
                            <br>Fixed some crashes which were supposed to be "out of memory" errors.
                            <br>Fixed a race condition with the New Image, Canvas Size, and Resize dialogs. If you typed
                            extremely fast you could cause a crash by typing a negative number and immediately pressing
                            OK or Enter.
                            <br>Fixed a File-&gt;Save dialog issue in Win7/Vista where it could ask you about
                            overwriting the wrong file.
                            <br>Paint.NET v3.5.2, released on January 4th, 2010
                            <br>This update resolves some feature disparities in the Text tool between GDI (XP) and
                            DirectWrite (Win7/Vista). It also improves overall performance, as well as the correctness
                            and quality of the Move Selected Pixels tool, the Image-&gt;Resize function, and the
                            Hue/Saturation adjustment.
                            <br>
                            <br>All font face variants (e.g., Arial vs. Arial Narrow) are now available with the Text
                            tool in Win7/Vista with DirectWrite.
                            <br>Bitmap font types (e.g. Courier, Terminal, Fixedsys) are now available with the Text
                            tool in Win7/Vista.
                            <br>Fixed some bad text kerning with the Text tool at small font sizes when antialiasing was
                            turned off.
                            <br>For the Image-&gt;Resize function, the quality, correctness, and performance of Bilinear
                            and Bicubic sampling modes have been improved. Super Sampling also has some performance
                            improvement.
                            <br>Improved the rendering quality for the Hue/Saturation adjustment. Also made a new icon
                            for it.
                            <br>Fixed many subtle rendering issues with the Move Selected Pixels tool. These were
                            apparent when flipping or rotating a selected area.
                            <br>Fixed: The Line/Curve tool was applying pixel snapping to the curve nodes, which caused
                            lines to "bend" when using the Shift key to constrain the angle.
                            <br>Fixed some extraneous CPU usage related to unnecessary or redundant thumbnail updates.
                            <br>Fixed a few dialogs that looked wrong with Aero glass with Remote Desktop or Virtual PC.
                            <br>Fixed a nasty memory leak with Flatten followed by Undo.
                            <br>Fixed some issues related to effects that took awhile to cancel. As it turns out,
                            drag-and-drop was enabled at this time, which easily lead to crashes or hangs.
                            <br>Some Win7 systems could not detect that .NET 3.5 SP1 was installed, even though it was.
                            A fallback detection function has been added.
                            <br>For plugin authors, the Effect class now has a pollable IsCancelRequested property. This
                            can be used to improve responsiveness for expensive OnSetRenderInfo() implementations which
                            are otherwise non-interruptible.
                            <br>For plugin authors, the Surface.FitSurface() method is now optimized to use multiple
                            threads, which improves performance.
                            <br>Paint.NET v3.5.1, released on November 19th, 2009
                            <br>This update adds a new feature for Windows 7 users, and fixes many small issues that
                            have been found since 3.5's release.
                            <br>
                            <br>New: For Windows 7, added taskbar progress reporting for long running operations
                            (effects, adjustments, Image-&gt;Resize, save, install)
                            <br>
                            <br>Made some corrections to the French translation
                            <br>Running setup with /auto will no longer launch Paint.NET when it's done
                            <br>Fixed an issue where Paste into New Image would refuse an image on the clipboard, even
                            if regular Paste would take it
                            <br>Fixed a race condition with Edit-&gt;Paste and Image-&gt;Resize whereby it would take up
                            100% CPU and take between 1 minute to 1 hour to finish
                            <br>Fixed an issues with Copy/Paste where it would leave an extra line of transparent pixels
                            on the left, top, right, and/or bottom edges
                            <br>Fixed lag with the paintbrush tool that was being seen on some systems
                            <br>Fixed some issues with the paintbrush and eraser tool being misaligned when zoomed in
                            <br>Fixed a crash that would happen at (seemingly) random times, such as after drawing with
                            the paintbrush tool, on some systems
                            <br>Fixed a minor and obscure rendering glitch with the Move Selected Pixels tool
                            <br>Fixed an issue with glass over Remote Desktop or Windows 7 Virtual PC
                            <br>Fixed a minor glitch whereby the "Unsaved Changes" confirmation dialog could never
                            finish rendering the image thumbnail if one of the Move tools was active
                            <br>Paint.NET v3.5, released on November 6th, 2009
                            <br>This release focused on improving performance reliability, reducing memory usage,
                            upgrading to the latest .NET Framework version, and refreshing the user interface for Aero
                            and glass (Windows 7 / Vista).
                            <br>
                            <br>New: Refreshed user interface with new icons and visual styling. On Windows 7 and Vista,
                            it is enhanced for Aero and "glass".
                            <br>
                            <br>New effect: Blurs -&gt; Surface Blur, by Ed Harvey
                            <br>New effect: Distort -&gt; Dents, by Ed Harvey
                            <br>New effect: Distort -&gt; Crystalize, by Ed Harvey
                            <br>New: Russian translation.
                            <br>Performance and memory usage have been extensively optimized throughout the entire
                            program.
                            <br>.NET Framework 3.5 SP1 is now required, which has many built-in performance
                            improvements.
                            <br>Disk space usage has been reduced by about 12MB by using NTFS compression on
                            installation files related to staging (.MSI) and diagnostics (.PDB).
                            <br>Compression for .PDN images has been improved.
                            <br>Effect dialog responsiveness has been improved.
                            <br>Images open much faster, especially on single CPU systems.
                            <br>Startup performance on most systems will be better by about 20%.
                            <br>Memory usage has been reduced when more than one image is open.
                            <br>Rendering quality has been greatly improved when zoomed in.
                            <br>The selection outline is no longer animated. Instead of "dancing ants", a
                            context-sensitive "XOR" stipple pattern is drawn. This has allowed for improved performance
                            and lowered CPU consumption (and longer battery life).
                            <br>The font manager for the Text tool has been completely rewritten, which fixes many
                            problems seen with crashes and missing fonts.
                            <br>On Windows XP, the Text tool has improved reliability and font selection (it uses GDI
                            instead of GDI+).
                            <br>On Windows 7, the Text tool will use DirectWrite (instead of GDI) which gives better
                            performance and greatly improved quality. On Windows Vista, you may install DirectX 11 to
                            enable this feature; otherwise GDI will be used.
                            <br>The toolbar font list has improved usability, rendering quality, and significantly
                            improved performance.
                            <br>The toolbar font list no longer requires an application restart to recognize newly
                            installed fonts.
                            <br>When many fonts are installed, both memory usage and startup performance have been
                            greatly improved.
                            <br>It is now drastically easier to move a very small selection.
                            <br>All installation prerequisites are now installed automatically, such as .NET and Windows
                            Installer.
                            <br>Updates are now downloaded in the background, and installed after you exit the
                            application. In previous versions, this was a foreground task and you could not use
                            Paint.NET while the update was downloaded.
                            <br>Added a "Utilities" menu. Updates, Languages, and Plugin Errors have been moved there.
                            <br>Added a "Manage Fonts" command to the Utilities menu. This will launch the built-in
                            Windows font control panel.
                            <br>Clicking the middle mouse button on an image thumbnail will now close the image.
                            <br>Improved the Unfocus effect.
                            <br>The DirectDraw Surface (.DDS) file type now allows you to select the resampling
                            algorithm for auto-generated mip-maps.
                            <br>A processor that supports SSE is now required (almost all CPUs purchased this decade
                            satisfy this).
                            <br>Fixed an issue with Gaussian Blur and its treatment of alpha values.
                            <br>Fixed a crash with the "Units" selector in the toolbar.
                            <br>Fixed a crash due to an overflow that prevented very large images from working (64-bit
                            only).
                            <br>Fixed many other miscellaneous glitches and crashes.
                            <br>The Korean translation has been removed. Sadly, we were unable to find the resources to
                            complete this.
                            <br>Paint.NET v3.36 Released: August 26th, 2008 - Download
                            <br>This is mostly a servicing release to make some small improvements and to fix a few
                            important bugs.
                            <br>
                            <br>Improved: Effect rendering should be a little faster now.
                            <br>Changed: Implemented some changes to the "Add Noise" effect that were suggested by a
                            forum member.
                            <br>Changed: The canvas background color is now always #c0c0c0.
                            <br>Changed: The auto-updater should now correctly detect .NET 3.5 and newer, which will
                            help to save bandwidth when Paint.NET v4.0 is released (it will require .NET 3.5).
                            <br>Fixed: Paint.NET now works on a system that has the .NET 3.5 SP1 "Client Profile"
                            installed.
                            <br>Fixed: When zoomed in and the cursor is to the top-left of the image (negative
                            coordinates), the ruler is now highlighted in the correct area.
                            <br>Fixed: The effect rendering system no longer sets the "Tag" property on the
                            configuration dialog.
                            <br>Fixed: Some incorrectly authored plugins would cause a crash when loading their support
                            details (author, copyright, etc.).
                            <br>Fixed: There was a bug in the color wheel for IndirectUI that caused it to show the
                            wrong values at initialization.
                            <br>Fixed: There was a performance problem for effects that used the IndirectUI color wheel
                            control.
                            <br>Fixed: In some rare cases, Paint.NET would crash while shutting down.
                            <br>Fixed: When using the "Fixed Ratio" feature of the Rectangle Selection tool, it would
                            crash if 0 was specified for both the width and height.
                            <br>Paint.NET v3.35 Released: July 7th, 2008
                            <br>This releases introduces a new Posterize adjustment, a new Intersect selection mode,
                            dramatically improved performance for selection editing, and several small bug fixes.
                            <br>
                            <br>New: Posterize adjustment, by Ed Harvey.
                            <br>New: Intersect selection editing mode.
                            <br>Improved: Dramatically improved selection editing performance for the Add and Subtract
                            modes (and also for Intersect). The performance used to be dependent on image size, and thus
                            was often unusable on images larger than 1024x768 pixels. It is now dependent only on
                            selection complexity (number of polygon edges) -- the improvement is generally between 3x
                            and 1000x.
                            <br>New: When holding Ctrl or Alt for a selection tool, the cursor now has a plus or minus
                            indicator.
                            <br>Changed: The canvas background is now a solid color instead of a gradient. The gradient
                            was causing certain tone misjudgments related to bright versus dark colors.
                            <br>Changed: Shortcut key for Sepia is now Ctrl+Shift+E. The shortcut for Posterize is now
                            Ctrl+Shift+P.
                            <br>Changed: Hotkeys for selection modes are now Left click for Replace, Control+Left click
                            for Add (union), Alt+Left click for Subtract (difference), Ctrl+Left click for Intersect,
                            and Ctrl+Right click for Invert (xor).
                            <br>Changed: When using a selection mode other than "replace", it will now draw the
                            selection outline so that you can see both the original and resulting selection areas.
                            Before, it would only draw the resulting selection area outline, which made modes such as
                            Intersect hard to use.
                            <br>Fixed: The Resize dialog had some rounding errors with the "Maintain aspect ratio"
                            feature, which caused a few discrepancies and even a spurious "out of memory" error.
                            <br>Fixed: Some quirks with the Color Wheel control for IndirectUI-based effect plugins.
                            <br>Fixed: Several miscellaneous and rare crashes.
                            <br>Fixed: The installer would display a bizarre error if a "blank" install folder was
                            attempted.
                            <br>Fixed: The installer now only accepts absolute path locations, instead of relative ones.
                            This fixes an ambiguity between where Paint.NET believes it is installing itself to, and the
                            directory that Windows Installer actually uses.
                            <br>Fixed: Sometimes pasting would result in a crash when certain types of malfored data
                            were on the clipboard.
                            <br>Fixed: It was possible to get around some of the protections imposed by the IndirectUI
                            system. This was causing instability with some effect plugins such as "Fern Fractal".
                            <br>Fixed: There were some issues with the implementation of "linked" sliders for effects
                            based on IndirectUI.
                            <br>Paint.NET v3.31 Released: May 1st, 2008 - Download
                            <br>This is mostly a servicing release to fix a few important bugs.
                            <br>
                            <br>New: Enabled integration with Window Clippings, which is a high quality screen capture
                            utility by Kenny Kerr.
                            <br>Fixed: Fixed a crash with the Open/Save dialogs if the Documents or Pictures directories
                            were either inaccessible or if the user did not have certain file system permissions.
                            <br>Changed / Fixed: The hotkey for Adjustments -&gt; Levels is now Ctrl+Shift+L instead of
                            Ctrl+Alt+L. This was preventing certain characters, such as the Polish 'ł', from being
                            typed.
                            <br>Paint.NET v3.30 Released: April 10th, 2008
                            <br>This release adds an Italian translation, a new "Fragment Blur" effect, and the ability
                            to save PNG images at 8- and 24-bit color depths. For developers, the IndirectUI system has
                            some new controls, some new constraint rules, and can now be used for file type plugins.
                            <br>
                            <br>New: Italian translation.
                            <br>New: Ability to save PNG's at 8- and 24-bit color depths.
                            <br>New: Ability to save BMP's at 8-bit color depth.
                            <br>New: "Auto-detect" bit-depth option for PNG, BMP, and TGA file types. It will analyze
                            the image and determine the lowest bit-depth that can still save the image without quality
                            loss.
                            <br>New: "Fragment" blur effect, by Ed Harvey
                            <br>New: The "Polar Inversion" distortion effect has been enhanced to allow changing the
                            rendering offset, and the behavior for "edge" pixels (clamp, reflect, or wrap).
                            <br>New: For developers, added a Color Wheel control to IndirectUI for use in effect
                            plugins.
                            <br>New: For developers, added ability to customize certain properties of the effect
                            configuration dialog via IndirectUI.
                            <br>New: For developers, IndirectUI can now be used to write configuration UI for file
                            types.
                            <br>New: For developers, IndirectUI has a new radio button control type for enumerations,
                            and some new property constraint rules.
                            <br>Changed: Most effects and adjustments, including plugins that use IndirectUI, have been
                            visually refreshed. The new look is cleaner and more compact. These changes are shown in
                            more detail at http://blog.getpaint.net/2008/03/10/cleaning-up-the-ui-for-paintnet-v330/
                            <br>Fixed: Various UI issues with the Levels adjustment.
                            <br>Fixed: When pasting text into the Text tool with Ctrl+V, it would hide the nub for
                            moving the text.
                            <br>Fixed: If the startup tool was set to the Zoom or Pan (Hand) tool, then the toolbar
                            would render incorrectly.
                            <br>Fixed: Thumbnails for PDN images now include transparency, which improves their
                            appearance in Windows Vista.
                            <br>Fixed: In some cases, an exponential property slider would get "stuck" at some values
                            when using up/down keyboard keys. This mostly affects some effect plugins.
                            <br>Fixed: When using keyboard navigation, sometimes the File menu would scroll its items
                            out of view.
                            <br>Fixed: Some crashes that were tracked down to out-of-bounds coordinate values in certain
                            effects.
                            <br>Fixed: The installer would fail if Paint.NET had never been installed before, and was
                            being installed to any non-default directory. This bug only affected version 3.22.
                            <br>Paint.NET v3.22 Released: January 12th, 2008 - Download
                            <br>This release fixes a few minor bugs and adds a new, much-needed Reduce Noise effect.
                            <br>
                            <br>New: "Reduce Noise" effect.
                            <br>Changed: Ctrl+W will now close Paint.NET if zero images are open.
                            <br>Fixed: In Windows XP, when launching web content, sometimes Internet Explorer was used
                            instead of the user's chosen default browser.
                            <br>Fixed: The Unfocus effect was not handling alpha values properly.
                            <br>Fixed: The Brightness / Contrast adjustment was only displaying its text in English.
                            <br>Fixed: The /auto parameter for the installer now correctly allows for an automated
                            installation. This was inadvertently broken in 3.20.
                            <br>Paint.NET v3.20 Released: December 12th, 2007
                            <br>This release adds numerous enhancements and tweaks to the built-in effects, a
                            re-organized Effects menu, a new and much easier system for effect plugin development,
                            better error handling for plugins, and the ability to draw Fixed Ratio and Fixed Size
                            selections with the Rectangle Select tool. It also includes the customary list of tweaks and
                            fixes.
                            <br>
                            <br>Rectangle Select tool can now draw selections based on a Fixed Size or Fixed Ratio
                            setting.
                            <br>
                            <br>
                            <br>The selection combination mode is now accessible from the toolbar (Replace, Add,
                            Subtract, Invert ("xor")).
                            <br>
                            <br>
                            <br>The "flood mode" for the Magic Wand and Paint Bucket tool are now accessible from the
                            toolbar (Continuous, or Global).
                            <br>
                            <br>
                            <br>Reorganized the Effects menu so that all effects are classified under submenus named
                            Artistic, Blurs, Distort, Noise, Photo, Render, and Stylize.
                            <br>Improved rendering quality for the Motion Blur effect.
                            <br>Enhanced the Radial Blur effect so that the center of blurring can be chosen, as well as
                            the quality.
                            <br>Enhanced the Zoom Blur effect so that the center of zooming can be chosen.
                            <br>Enhanced the Bulge distortion effect so that the center of "bulging" can be chosen.
                            <br>Enhanced the Frosted Glass distortion effect in several ways: 1) performance has been
                            improved from between 1,000% to 10,000% depending on image size and property settings, 2)
                            the scatter radius can now be set up to 200 pixels, 3) a "minimum" scatter radius can be
                            chosen, 4) a smoothness setting is now available.
                            <br>Enhanced the Tile Reflection distortion effect by adding a Quality property.
                            <br>Enhanced the Twist distortion effect by 1) allowing counter-clockwise twisting, 2)
                            allowing the size of the twisted area to be configured, 3) allowing the location/center of
                            twisting to be chosen.
                            <br>Enhanced the Add Noise effect by adding a "coverage" property.
                            <br>New Mandelbrot Fractal and Julia Fractal render effects.
                            <br>New IndirectUI system for plugin authors so that they can develop much more
                            sophisticated effect configuration dialogs with a fraction of the amount of work that used
                            to be required.
                            <br>If an effect plugin crashes, it is much more likely that Paint.NET will be able to
                            recover from the error.
                            <br>The option to restart Paint.NET will then be provided as a recommended course of action.
                            <br>If an effect plugin fails to load, or is blocked from loading, then a "View Plugin Load
                            Errors..." item will be added to the File menu which can be clicked on to show the error
                            and/or diagnostic information.
                            <br>Improved the cursors for the Magic Wand and Paint Bucket tools.
                            <br>Ctrl+Alt+0 now works for View-&gt;Actual Size (aka, "Zoom to 100%"), which is a shortcut
                            key that other software uses (e.g., Photoshop).
                            <br>Updates are now installed faster by only creating one System Restore point instead of
                            two (it used to implicitly create one for uninstall, then one for the reinstall).
                            <br>Lots of little bug fixes.
                            <br>Paint.NET v3.10 Released: August 23rd, 2007
                            <br>This release adds two new effects originally written by David Issel ("BoltBait"),
                            support for the DDS filetype originally written by Dean Ashton, as well as many small bug
                            fixes and some visual fit and finish.
                            <br>
                            <br>New: Soften Portrait effect, by David Issel, http://www.BoltBait.com .
                            <br>New: Ink Sketch effect, by David Issel, http://www.BoltBait.com .
                            <br>New: DirectDraw Surface (DDS) file format support, by Dean Ashton,
                            http://www.dmashton.co.uk/ . Improved from the original source code by optimizing the DXT
                            compression library ("Squish") to take advantage of multiple cores / processors.
                            <br>New: "Paint.NET Search", available from the Help menu (shortcut key is Ctrl+E), allows
                            you to search for Paint.NET help, forum posts, tutorials, plugins, and other related
                            material: http://searchpaint.net (Note: This feature is only available in English.)
                            <br>Improved: Visual fit-and-finish for the Layers window.
                            <br>Improved: Visual fit-and-finish for the close / 'X' button on image thumbnails.
                            <br>Improved: Small (about 5-10%) performance improvements for some effects such as Oil
                            Painting, Frosted Glass, and Gaussian Blur.
                            <br>Improved: Increased max brush size to 500, as per forum members request.
                            <br>Improved: Expanded list of available font sizes up through 288.
                            <br>Changed: The keyboard shortcut key for the Color Picker is now 'k'. This makes it so
                            that the toolbar option, "After click: Switch to previous tool", is not useless for those
                            using the keyboard shortcuts.
                            <br>Fixed: In some cases, undoing an action that removed a layer would result in the
                            un-removed layer not showing up until you resized the Layers window ("ghost layers").
                            <br>Fixed: Pressing F1 from the main window no longer launches the online help in two
                            browser tabs.
                            <br>Fixed: Adding a new layer now adds it above the currently active layer, instead of at
                            the very top of the layer list.
                            <br>Fixed: Merge Down now activates the merged layer instead of the one above it.
                            <br>Fixed: In Vista, clicking on a URL link from the installer will no longer launch the web
                            browser with inherited, elevated privileges.
                            <br>Fixed: Pressing Ctrl+[ no longer cancels out of drawing a line/curve, but instead
                            decreases the brush size by 5 as expected.
                            <br>Fixed: Ctrl+clicking on the brush size +/- buttons now changes the brush size in
                            increments of 5.
                            <br>Fixed: Save Configuration dialog would "creep downward" from its last position every
                            time it was opened again.
                            <br>Fixed: TGA codec now saves the # of alpha bits to the image descriptor byte. This was
                            causing some other applications to load TGA files saved with Paint.NET as solid black
                            images.
                            <br>Fixed: Clicking the 'X' to close the Layer Properties dialog was not reverting changes
                            made to the layer while the dialog was open.
                            <br>Fixed: Installation will not proceed unless Paint.NET is closed, and will also not allow
                            Paint.NET to be opened until installation is completed. This helps to ensure a fully
                            coherent and complete installation or update.
                            <br>Fixed: If a file failed to open, and there were no open images, and the user pressed
                            either the Zoom In or Zoom Out toolbar buttons, then Paint.NET would crash.
                            <br>Fixed: In Vista, it was possible to crash the Save As dialog by typing a filename that
                            was too long.
                            <br>Fixed: In Vista, it was possible to crash the updater if you let the UAC prompt
                            time-out.
                            <br>Fixed: It was possible to crash Paint.NET on some systems by clicking on a tool in the
                            Tools window while the "Save As" dialog was open.
                            <br>
                            <br>v3.08 Released: June 1st, 2007
                            <br>This is mostly a service release that fixes some bugs, while also improving keyboard /
                            accessibility cues for some dialogs.
                            <br>Fixed: Pasting an image from Office 2003 applications now works (e.g. Excel 2003
                            graphs).
                            <br>Fixed: Some dialogs were not indicating which command button was the default. These
                            buttons now have a highlight to indicate which one will be activated if the user presses
                            Enter or Space.
                            <br>Fixed: Some minor keyboard navigation issues with task dialogs
                            <br>Fixed: Performance issue with the File-&gt;Acquire submenu taking a long time to appear
                            <br>Fixed: Window activation issue when the Print wizard was finished / closed
                            <br>Fixed: Crash when there was 1 image open and the user pressed Ctrl+Q and then Ctrl+W
                            <br>Fixed: Minor performance issue if the user had 1 modified image open and then canceled
                            the "Save changes?" dialog
                            <br>Fixed: Misbehaving filetype factory implementations (plugins) will no longer cause a
                            crash
                            <br>
                            <br>v3.07 Released: May 8th, 2007
                            <br>This update enhances the Line/Curve tool, significantly reduces the download size, and
                            fixes some bugs related to opening and saving files in Windows Vista.
                            <br>New: Line/Curve tool has been enhanced to allow drawing arrowheads, and to draw with
                            various dashed- and dotted- styles.
                            <br>New: Image tab thumbnails now have an indicator if the respective image has unsaved
                            changes (an orange asterisk is shown).
                            <br>Improved: The Save Configuration dialog (choose JPEG quality, etc.) now allows you to
                            maximize it. It also remembers its relative location and size.
                            <br>Changed: The help file / documentation is now hosted online. This has reduced the
                            download size by more than 3 MB, and will also allow us to provide translations without
                            ballooning the size of the download (each language would have added between 2 and 4MB).
                            <br>Changed: The "image list button" (downward triangle) is also shown when only 1 image is
                            open (it used to only display if 2 or more images were open). This is being done for the
                            sake of consistency.
                            <br>Fixed: Some operations would reset the selected layer to the first/lowest layer. This
                            selection is now preserved.
                            <br>Fixed: The Image-&gt;Rotate commands no longer hang if a selection was active.
                            <br>Fixed: Several problems have been fixed within our implementation surrounding the new
                            Vista Open/Save dialogs. This includes: opening an image from an http:// source, opening
                            images from a digital camera that is not mapped to a file system path (such as a drive
                            letter), the Save dialog not always prompting you about overwriting an existing file, and
                            many corner cases that previously caused crashes.
                            <br>
                            <br>v3.05 Released: March 29th, 2007
                            <br>This is a minor update that adds a new effect, improves certain parts of the user
                            interface, and fixes a few minor bugs.
                            <br>New: Pencil Sketch effect
                            <br>New: In Windows Vista, the new-style Save/Open dialogs are used. Among other things,
                            this enables Search functionality.
                            <br>Changed: The View-&gt;Units, Image-&gt;Flip, Image-&gt;Rotate, and Layers-&gt;Flip
                            submenus have been "flattened" (their commands were moved out into the View, Image, Image,
                            and Layers menus respectively)
                            <br>Improved: Download size reduced by about 300 KB by using PNGOUT
                            <br>Improved: Some uses of confusing "MessageBox" style dialogs have been changed to a much
                            friendlier "TaskDialog" style interface
                            <br>Improved: When changing the language, Paint.NET can now restart itself automatically
                            <br>Improved: Better performance for Move Selected Pixels tool for quad-core systems. This
                            issue is documented and explained here,
                            http://blogs.msdn.com/rickbrew/archive/2007/03/01/paint-net-many-core-performance-scaling-analyzed.aspx
                            <br>Removed: The "Clear History" button has been removed because it was not very useful
                            <br>Fixed: Sometimes the Colors window would get "lost" between sessions of Paint.NET
                            <br>Fixed: Stack-overflow crash when using certain effects, such as Gaussian Blur, on very
                            large images with certain settings (such as a 200 pixel radius)
                            <br>Fixed: When cancelling the multi-image Unsaved Changes dialog, the input focus was
                            sometimes confused
                            <br>Changed: Renamed PdnLib.dll to PaintDotNet.Core.dll
                            <br>Fixed: Very rare race condition in background thumbnail renderer
                            <br>v3.01 Released: February 26th, 2007 - Download
                            <br>This is a small update that fixes a few bugs that have been found since 3.0 was
                            released.
                            <br>
                            <br>Fixed: Crash when trying to save a palette with a blank name
                            <br>Fixed: Changing an image's DPI resolution did not set its "dirty" flag (you would not be
                            asked to save changes)
                            <br>Fixed: Error messages at startup were covered by the splash screen
                            <br>Fixed: Crash when a modal dialog was open (such as an effect) when the user tried to
                            logoff/restart/shutdown Windows, and they chose to save their images
                            <br>Mitigated some CPU usage issues when the app was minimized and a complex selection was
                            active
                            <br>v3.0 Released: January 26th, 2007
                            <br>This major release introduces a new multi-document interface (MDI), availability in 8
                            languages, a highly-requested interactive gradient tool, four new effects, a user-definable
                            color palette, lower disk space usage for scratch files, and a generally cleaner and
                            improved user interface.
                            <br>
                            <br>What's new in Paint.NET v3.0?
                            <br>
                            <br>Simple and intuitive tab-based multi-document user interface
                            <br>
                            <br>
                            <br>Now available in 8 languages: English, Chinese (Simplified), French, German, Japanese,
                            Korean, Portuguese (Brazil), and Spanish
                            <br>
                            <br>
                            <br>Interactive Gradient Tool that makes it very easy to draw and then fine-tune placement
                            and coloring of a gradient.
                            <br>
                            <br>
                            <br>User-definable color palette (as opposed to just the color wheel)
                            <br>
                            <br>
                            <br>New effects: Clouds, Median, Unfocus, Outline, and an improved Sharpen
                            <br>More intuitive and more powerful toolbar
                            <br>Generally improved and cleaner user interface
                            <br>History files are now compressed to save disk space, reduce disk activity, and improve
                            performance.
                            <br>"Merge Down" layer command
                            <br>Please note that Windows 2000 is no longer supported. Paint.NET v3.0 will not install
                            unless your operating system is Windows XP SP2 or newer.
                            <br>
                            <br>
                            <br>Paint.NET v2.7x
                            <br>v2.72 Released: August 31st, 2006
                            <br>This small release adds a new effect and fixes a few small bugs.
                            <br>New effect: Zoom Blur
                            <br>Fixed: DPI was not being saved or loaded correctly for file types other than PDN and
                            JPEG
                            <br>Fixed: Text Tool now works with Alt+#### special character entry without moving the
                            cursor
                            <br>Fixed: Loading PNG images with alpha was often resulting in incorrect, off-by-1 color
                            values
                            <br>v2.70 Released: August 2nd, 2006
                            <br>This is a small interim release that includes many of the popular effect plugins we have
                            written that users have enjoyed using with Paint.NET v2.6x. We have decided to release this
                            as a ".1" update now so that more users may benefit from these plugins, as opposed to
                            waiting until the final release of v3.0 to include them (which could be awhile).
                            <br>
                            <br>With this release we have also refreshed Paint.NET's system requirements. We now list
                            256 MB as the minimum memory required instead of 128 MB. This is in line with what we have
                            seen to be a more reasonable minimum system for using Paint.NET. Also, Windows XP users must
                            now have SP2 installed (SP1 was required before), Windows 2000 users must have SP4 installed
                            (SP3 was required before), and Windows Server 2003 users must have SP1 installed (no SP was
                            required before).
                            <br>
                            <br>New effect: Glow
                            <br>New effect: Bulge
                            <br>New effect: Polar Inversion
                            <br>New effect: Tile Reflection
                            <br>New effect: Twist
                            <br>Paint.NET v2.6x
                            <br>v2.64 Released: July 8th, 2006
                            <br>This small updates fixes a few minor bugs, and improves Windows Vista compatibility. As
                            a bonus, it also adds much better GIF save quality.
                            <br>
                            <br>Improved GIF save quality by implementing Floyd-Steinburg error diffusion algorithm
                            <br>Printing now works in Windows Vista
                            <br>Fixed a startup performance problem on some systems that was an artifact of the way the
                            .NET Framework was verifying Authenticode signatures as part of its assembly loading process
                            <br>Executable files now have UAC manifests to ensure proper execution privilege and to
                            disable file and registry virtualization in Windows Vista
                            <br>v2.63 Released: June 4th, 2006
                            <br>This small update fixes some more relatively minor bugs, and makes the built-in updater
                            much more convenient in Windows Vista.
                            <br>
                            <br>Built-in updater now works in Vista without having to use "Run as Administrator"
                            beforehand (UAC permission is still required to install updates)
                            <br>Fixed a color intensity calculation that had Red and Blue swapped (affects
                            Brightness/Contrast adjustment, and some plugins)
                            <br>Fixed .PDN images with transparency having a black background in their Explorer
                            thumbnail
                            <br>Fixed crash when an image has bizarre DPI settings (such as 6 billion DPI)
                            <br>Fixed crash when an image has an invalid resolution unit specified (neither pixels,
                            inches, nor centimeters)
                            <br>Fixed a few rare race conditions which resulted in crashes
                            <br>Fixed a rare crash with the history
                            <br>Fixed crashlog being created when the updates dialog appears over another modal dialog
                            <br>Fixed crashlog not reporting application version with certain damaged installations
                            <br>Placed a clickable Windows Live OneCare ad in the Setup wizard that expires on July
                            10th, 2006
                            <br>v2.62 Released: May 10th, 2006 - Download
                            <br>This small update fixes some bugs, and improves the user experience on some Windows
                            Vista systems.
                            <br>
                            <br>Small icon (16x16) is brand new, redesigned so that it is clearer
                            <br>Application resolution is no longer virtualized in high-DPI mode in Windows Vista
                            <br>Fixed race-condition related crash with Edit-&gt;Paste and Move Selected Pixels tool
                            ("Object is in use elsewhere")
                            <br>Fixed some font related crashes that occur when standard fonts are corrupt or missing
                            <br>Fixed a crash that sometimes occurs when trying to save files whose name begins with a
                            period
                            <br>Fixed a rare division-by-zero crash in the Clone Stamp
                            <br>Fixed rare crash related to scanning
                            <br>Mitigated rare crash that can happen in various places, ("GetRegionData returned false,
                            GetLastError() = 6")
                            <br>Improved crash log reporting
                            <br>v2.61 Released: March 29th, 2006
                            <br>This small update fixes a few uncommon bugs, and adds a "Donate" item to the Help menu
                            that links to our donation page.
                            <br>
                            <br>Fixed crash when clicking File-&gt;New when there is a malformed image in the clipboard
                            <br>Fixed several crashes related to pressing Ctrl+Z (Undo) or Ctrl+Y (Redo) before
                            releasing the mouse button while still drawing
                            <br>Fixed Zoom Tool "haze" remaining after pressing Ctrl+Z before releasing the mouse button
                            <br>Fixed uninstaller not removing Start-&gt;Programs menu shortcut
                            <br>Fixed "Auto" button in Adjustments-&gt;Levels not updating one of its sliders
                            <br>Fixed a few small plugin API problems
                            <br>Fixed a race condition in the file loading code related to EXIF tags
                            <br>Added "Donate" to Help menu
                            <br>v2.6 Released: February 24th, 2006
                            <br>This release is an upgrade of v2.5 that utilizes the brand new .NET Framework v2.0
                            runtime. It introduces full 64-bit support, an aesthetically updated user interface, better
                            performance, a new "Curves" adjustment, and seven new layer blend modes.
                            <br>
                            <br>What's new in Paint.NET v2.6?
                            <br>
                            <br>Full 64-bit support, for both x64 and Itanium systems
                            <br>New "Curves" adjustment for editing an image's color curves
                            <br>Seven new layer blend modes: Color Burn, Color Dodge, Reflect, Glow, Overlay, Negation,
                            and Xor
                            <br>Aesthetic improvements to the entire user interface
                            <br>Better performance, especially for 64-bit systems
                            <br>Zooming, esp. with the mouse wheel, has been enhanced
                            <br>Rewritten layer composition engine is now mathematically correct, and faster
                            <br>Deployment via AD/GPO is now much easier (use /createMsi with setup package)
                            <br>User interface now works correctly in high-DPI (120dpi, 144dpi, 196dpi)
                            <br>Layers window list is no longer "upside down"
                            <br>Upgraded to use .NET Framework 2.0
                            <br>Many other improvements and fixes
                            <br>Paint.NET v2.5
                            <br>Released: November 26th, 2005 - Download
                            <br>
                            <br>The major goals of this release were to improve performance, expand selection support to
                            be much more useful and powerful, provide support for localization to other languages, and
                            to have an easier way for users to have the latest version (update manager). Other features
                            added include the ability to work with measurements in inches and centimeters, a 3D
                            Rotate/Zoom effect, Sepia adjustment, Radial Blur and Add Noise effects, GIF transparency
                            support, TGA file format support, file format plugin support, and a refined Text tool.
                            <br>
                            <br>What's new in Paint.NET v2.5?
                            <br>
                            <br>Faster performance and lower memory usage
                            <br>Full flexibility for scaling, rotating, and moving selections and selected pixels
                            <br>Ability to subtract from and add to selections
                            <br>Internationalization (I18N) support
                            <br>Officially available in German
                            <br>Line / Curve tool lets you draw spline and Bézier curves
                            <br>Ability to work in measurements of inches and centimeters
                            <br>3D Rotate / Zoom effect lets you rotate, tilt, and tile images at various perspectives
                            <br>Radial Blur and Add Noise effects
                            <br>Sepia adjustment
                            <br>Improved Text Tool, including higher quality font rendering
                            <br>GIF transparency support
                            <br>TGA file format support
                            <br>Greater extensibility with a brand new File Format API
                            <br>Simpler, faster setup wizard
                            <br>Update manager simplifies getting the latest version
                            <br>Cleaner user interface with none of the annoying flickering of past releases
                            <br>Many other changes, improvements, and fixes
                            <br>Paint.NET v2.1
                            <br>v2.1b Released: May 12th, 2005 - Download
                            <br>This small updated fixes a crash when resizing an image with a new width but the same
                            height.
                            <br>
                            <br>v2.1a Released: May 5th, 2005
                            <br>This small update fixed a few crashes that people were experiencing related to the
                            "Open" and "Save As" dialogs. If you are not experiencing these crashes with v2.1 then you
                            do not need to download this update.
                            <br>
                            <br>v2.1 Released: April 30th, 2005
                            <br>The major goals of this release were to improve performance, refine the user interface
                            and experience, and to support some highly requested features such as PNG transparency
                            support and JPEG quality configuration. To summarize, Paint.NET v2.1 is much faster, more
                            compatible, and produces better quality images than v2.0. It is a highly recommended
                            upgrade.
                            <br>
                            <br>Many bug fixes and miscellaneous user interface tweaks.
                            <br>Installation via Group Policy is now supported.
                            <br>Rendering quality, usage, and performance of selections is improved.
                            <br>Much better performance all around.
                            <br>Magic Wand selection tool.
                            <br>Ellipse/circle selection tool.
                            <br>PNG transparency is now supported.
                            <br>GIF save quality significantly improved.
                            <br>JPEG quality selector and preview, and file size preview.
                            <br>Upgraded PDN file format to support very large images.
                            <br>Thumbnails are now shown for .PDN files in Windows Explorer.
                            <br>Much higher quality rendering when zooming out.
                            <br>Background layer is no longer "locked".
                            <br>EXIF data is now preserved for supporting file formats.
                            <br>Lower memory usage. History items are now saved to disk instead of completely stored in
                            memory.
                            <br>Better Tablet PC support. Also, Ink isn't used unless you have a Tablet PC; this has
                            increased compatibility and performance on regular systems.
                            <br>Ability to resize image based on a percentage.
                            <br>Brand new image resampling routines for Image-&gt;Resize menu item (no more transparent
                            borders).
                            <br>No more flickering in the UI.
                            <br>More optimizations for multiprocessor and multicore systems.
                            <br>Startup time is greatly reduced.
                            <br>
                            <br>Paint.NET v2.0
                            <br>Released: December 17th, 2004
                            <br>This was the release that was Slashdotted. Many important features were added and the
                            stability of the product was increased.
                            <br>Windows 2000 Compatible
                            <br>Levels Adjustments
                            <br>Auto Levels adjustment
                            <br>Clone Tool
                            <br>Color Replace Tool
                            <br>Zoom Tool
                            <br>Edge Detect Effect (Developed by Chris Crosetto)
                            <br>Relief Effect (Developed by Chris Crosetto)
                            <br>New emboss effect (Developed by Chris Crosetto)
                            <br>New oil painting effect
                            <br>New Frosted glass effect
                            <br>Red Eye removal effect
                            <br>Grid Mode when zoomed in close
                            <br>Help text for each tool displayed on the status bar
                            <br>Import Image to New Layers
                            <br>Variable zoom (not constrained to powers-of-2)
                            <br>Moving a selection makes the marching ants disappear
                            <br>Ability to adjust Hue / Saturation
                            <br>Ink support (for tablet PC users)
                            <br>Additional keyboard shortcuts
                            <br>Subtraction/difference blend operation for layers
                            <br>Image to auto zoom until fit inside window
                            <br>Tolerance Slider for adjustments for paint bucket and color replace
                            <br>Cursor transitions for tool actions
                            <br>Mouse positioning using keyboard arrows
                            <br>Limit history length
                            <br>
                            <br>Paint.NET v1.1
                            <br>Released: October 1st, 2004
                            <br>This release included many user interface tweaks and bug fixes.
                            <br>New Effect: "RotoZoomer" which can perform arbitrary angle rotation, and zooming.
                            <br>More responsive Effect preview rendering.
                            <br>Faster application startup time.
                            <br>"Open Recent" menu keeps track of the last 8 images you worked with, along with a
                            thumbnail for each.
                            <br>Selecting an area now draws an outline along with the blue highlight.
                            <br>Layer Properties now visually previews and updates all properties in real time without
                            having to press the "Apply" button.
                            <br>Invert and Desaturate are put into the Layers -&gt; Adjustments menu, along with a new
                            adjustment called "Brightness &amp; Contrast."
                            <br>Better performance when running in a Remote Desktop session by way of disabling dialog
                            box / toolform transparency.
                            <br>Zoom works correctly now: when you zoom in or out, the image will be centered to the
                            intuitively correct location.
                            <br>Lower memory usage and better resource usage in general.
                            <br>"Paste" now works with the Text tool.
                            <br>The location that images are pasted to is more intuitive in some scenarios.
                            <br>Improved "History" toolform user interface.
                            <br>User interface upgraded to make full use of XP themes. In v1.0, many dropdown boxes and
                            "updowns" had a Win2K/OfficeXP look to them.
                            <br>Other miscellaneous user interface tweaks.
                            <br>Many "under the hood" improvements, tweaks, bug fixes and refactorizations.
                            <br>New file format. Paint.NET v1.1 stores files with a ".pdn" extension which is not
                            compatible with Paint.NET v1.0's ".lbmp" extension.
                            <br>Extensibility! After you install the program, check out the "RotoZoomerSource.zip" for
                            an example of how to write an Effect plugin. You will need Visual Studio 2003 .NET to write
                            a new plugin. No other types of plugins are supported for v1.1.
                            <br>
                            <br>Paint.NET v1.0
                            <br>Released: May 6th, 2004
                            <br>The original project that started it all. This was completed in 15 weeks as an
                            undergraduate senior design project at WSU, and was 36,000 lines of code.</p>
                        <hr class="line">
                    </div>
                </div>
            </div>
        </section>
    </Layout>
</template>

<script>
    export default {
        metaInfo: {
            title: 'Roadmap'
        }
    }
</script>