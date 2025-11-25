=== Glacial AI Share Buttons ===
Contributors: Billy, Jamieson, Greg, Denmark
Tags: ai, share, buttons, chatgpt, claude, perplexity, grok, google ai
Requires at least: 5.0
Tested up to: 6.4
Requires PHP: 7.4
Stable tag: 1.3.2
License: GPLv2 or later
License URI: https://www.gnu.org/licenses/gpl-2.0.html

Add AI-powered share buttons at the end of blog posts to help readers explore content with various AI services.

== Description ==

Glacial AI Share Buttons is a WordPress plugin that adds share buttons for popular AI services at the end of your blog posts. This helps readers quickly analyze and summarize your content using their preferred AI tool.

**Features:**

* Injects AI share buttons at the end of blog post content
* Supports 6 popular AI services: Google AI Mode, ChatGPT, Perplexity, Claude, Grok, and Meta AI
* Custom AI tool repeater feature to add unlimited custom AI services
* Custom URL configuration for each AI service
* Real-time URL validation with client-side and server-side protection
* Enhanced security with input sanitization and SQL injection protection
* Customizable button section title
* Individual button toggle controls in admin settings
* Flexible per-post controls with both "Show" and "Hide" options for maximum customization
* Global "Add AI buttons on ALL posts" setting for site-wide control
* Custom post type selector to choose which content types display AI buttons
* Responsive Flexbox layout that adapts to different screen sizes with optimized mobile layout (2 columns on mobile)
* Theme-aware styling that inherits your theme's button styles
* Accessibility features including high contrast and reduced motion support
* Dark mode support

**Supported AI Services:**

* Google AI Mode
* ChatGPT
* Perplexity
* Claude
* Grok
* Meta AI
* Custom AI tools (via repeater feature)

== Installation ==

1. Upload the plugin files to the `/wp-content/plugins/glacial-ai-share-buttons` directory, or install the plugin through the WordPress plugins screen directly.
2. Activate the plugin through the 'Plugins' screen in WordPress
3. Go to Settings > Glacial AI Share Buttons to configure the plugin
4. Set your preferred title and enable/disable individual buttons
5. The buttons will automatically appear at the end of your blog posts

== Frequently Asked Questions ==

= How do I customize the button section title? =

Go to Settings > Glacial AI Share Buttons in your WordPress admin and modify the "Button Section Title" field.

= Can I control the buttons on specific posts? =

Yes! When editing a post, you'll find an "AI Share Buttons" meta box in the sidebar with two options:
- "Show AI buttons on this post" - Forces buttons to appear on this specific post
- "Hide AI buttons on this post" - Prevents buttons from appearing on this specific post

You can also use the global "Add AI buttons on ALL posts" setting in the plugin settings to control the default behavior site-wide.

= Which AI services are supported? =

The plugin supports Google AI Mode, ChatGPT, Perplexity, Claude, Grok, and Meta AI. You can also add custom AI tools using the repeater feature and configure custom URLs for each service. You can enable/disable each service individually in the settings.

= Will the buttons work with my theme? =

Yes! The plugin uses CSS that inherits your theme's button styling and includes responsive design that works with most themes.

= Are the buttons accessible? =

Yes, the plugin includes accessibility features like high contrast mode support, reduced motion support, and proper semantic HTML.

= How do I add custom AI tools? =

Use the repeater feature in the plugin settings to add unlimited custom AI services. You can configure the button name, URL, and icon for each custom AI tool.

= Can I customize the URLs for AI services? =

Yes! You can configure custom URLs for each AI service in the plugin settings, allowing you to use specific prompts or parameters for your content.

= How does URL validation work? =

The plugin includes comprehensive URL validation that works in real-time. Invalid URLs are prevented from being saved, and you'll see clear error messages for any issues. The validation checks for proper URL format and ensures URLs start with http:// or https://.

= Is my data secure? =

Yes! The plugin uses WordPress's built-in security functions and includes protection against SQL injection attacks. All user input is properly sanitized and validated before being stored.

= Can I choose which post types display the AI buttons? =

Yes! In the Glacial AI Share Buttons settings, you'll find a "Post Types" section where you can select which content types should display the AI share buttons. You can choose from Posts, Pages, Resources, Webinars, or any custom post types on your site. By default, only Posts are selected to maintain backward compatibility.

== Screenshots ==

1. Admin settings page showing button toggles, title field, and custom AI tool repeater
2. Post edit screen showing the exclude option meta box
3. Frontend display of AI share buttons on a blog post
4. Custom AI tool configuration interface

== Changelog ==

= 1.3.2 =
* **Post Type Filtering**: Improved post type selector to exclude system and data post types that aren't meant for displaying share buttons
* **Smart Post Type Detection**: Added intelligent filtering to only show publicly queryable content post types
* **Excluded System Post Types**: Automatically filters out structured data, reviews, collections, and other system post types from the settings page
* **Enhanced User Experience**: Settings page now only displays relevant content post types (Posts, Pages, Doctors, Locations, etc.) instead of all registered post types

= 1.3.1 =
* **Flexbox Layout Implementation**: Replaced CSS Grid with Flexbox for better responsive behavior
* **Flexible Button Sizing**: Buttons now use `flex: 1 1 calc(33.333% - var(--ai-gap-sm))` for 3 buttons per row on desktop
* **Automatic Wrapping**: Buttons automatically wrap based on available space using `flex-wrap: wrap`
* **Minimum Width Protection**: Added `min-width: 180px` to prevent buttons from becoming too narrow
* **Container Flexibility**: Layout works perfectly regardless of parent container width (60%, 100%, etc.)
* **Improved Responsiveness**: Better adaptation to different screen sizes and container widths

= 1.3.0 =
* **Reversed Logic & Enhanced Control**: Completely reversed the default behavior - AI buttons are now hidden by default and must be explicitly enabled
* **Global "Add AI buttons on ALL posts" Setting**: New admin checkbox to enable AI buttons on all posts site-wide
* **Dual Per-Post Controls**: Added both "Show AI buttons on this post" and "Hide AI buttons on this post" options for maximum flexibility
* **Smart Conflict Resolution**: JavaScript prevents both show/hide options from being checked simultaneously, with "Hide" taking precedence
* **Enhanced User Experience**: Clear visual feedback and intuitive interface for managing button display
* **Backward Compatibility**: Existing installations will maintain their current behavior while new installations use the new logic
* **Improved Documentation**: Updated FAQ section to explain the new control options and global settings

= 1.2.3 =
* **Custom Post Type Selector**: Added new admin setting to select which post types display AI share buttons
* **Enhanced Flexibility**: Users can now choose to display buttons on Posts, Pages, Resources, Webinars, or any custom post type
* **Improved Admin Interface**: New "Post Types" field in settings with checkboxes for all available post types
* **Backward Compatibility**: Default behavior remains unchanged (Posts only) for existing installations
* **Meta Box Integration**: Hide/show toggle now appears on all selected post types
* **Google AI URL Update**: Updated Google AI button to use Google Search with UDM parameter (https://www.google.com/search?udm=50&q=) for better compatibility, as Gemini doesn't support direct URL query parameters
* **Button Label Update**: Changed Google AI button label from "Google AI" to "Gemini" for better brand alignment

= 1.2.2 =
* **Default Icon Update**: Changed the default icon for additional AI tools from generic icon to sparkle emoji (✨) in SVG format for better visual appeal and consistency
* **Enhanced Custom AI Tools**: Improved the visual representation of custom AI services with the new sparkle icon as the default option

= 1.2.1 =
* **Google AI URL Update**: Updated Google AI button to use Google Search with UDM parameter (https://www.google.com/search?udm=50&q=) for better compatibility
* **Enhanced Security**: Added comprehensive URL validation with both client-side and server-side protection
* **SQL Injection Protection**: Implemented robust security measures to prevent SQL injection attacks
* **Real-time Validation**: Added live URL validation with immediate feedback for users
* **Data Sanitization**: Enhanced input sanitization and validation throughout the plugin
* **Mobile Layout Optimization**: Updated mobile flexbox layout to use 2 columns for better button arrangement on smaller screens

= 1.2.0 =
* **Meta AI Integration**: Added support for Meta AI service with dedicated button and URL configuration
* **Custom AI Tool Repeater**: New repeater feature allowing users to add unlimited custom AI services
* **Custom URL Configuration**: Enhanced URL customization for all AI services, including custom prompts and parameters
* **Improved Admin Interface**: Updated settings page with intuitive repeater controls for custom AI tools
* **Enhanced Flexibility**: Users can now configure button names, URLs, and icons for custom AI services

= 1.1.0 =
* **Enhanced Theme Integration**: Buttons now inherit your website's theme styling using the `ui-button` class for seamless design consistency
* **Improved Flexbox Layout**: Updated to use flexbox with flexible sizing for optimal button arrangement - 3 buttons on the first row, 2 buttons on the second row
* **Authentic Brand Logos**: Replaced generic icons with official brand SVG logos for all AI services
* **Smart Post Type Filtering**: Buttons now only appear on blog posts, automatically excluding other post types (pages, custom post types, etc.)
* **Default Button Configuration**: All AI service buttons are now enabled by default for immediate functionality
* **Refined Code Structure**: Improved code organization with better comments and cleaner architecture

= 1.0.0 =
* Initial release
* Support for 5 AI services
* Admin settings page
* Per-post exclude option
* Responsive Flexbox layout
* Theme integration
* Accessibility features

== Upgrade Notice ==

= 1.3.2 =
Post type filtering update that automatically excludes system and data post types from the settings page. The post type selector now only shows relevant content post types, making it easier to configure which content types display AI share buttons.

= 1.3.1 =
Layout update with improved flexbox implementation for better responsive behavior and container flexibility. Buttons now automatically wrap and adapt to any container width while maintaining optimal sizing.

= 1.3.0 =
Major update with reversed logic and enhanced control options. AI buttons are now hidden by default, giving you complete control over where they appear. New global "Add AI buttons on ALL posts" setting and dual per-post controls (Show/Hide) provide maximum flexibility. Includes smart conflict resolution and improved user experience.

= 1.2.3 =
Major update with custom post type selector functionality. Now you can choose which content types display AI share buttons - perfect for sites with multiple content types like blogs, resources, and webinars. Enhanced flexibility with backward compatibility maintained.

= 1.2.1 =
Security and functionality update with Google AI URL fix (now uses Google Search with UDM parameter), enhanced validation, improved security measures, and mobile layout optimization. Includes real-time URL validation, SQL injection protection, and better mobile button arrangement.

= 1.2.0 =
Major update with Meta AI integration, custom AI tool repeater feature, and enhanced URL customization. Now supports unlimited custom AI services with full configuration options.

= 1.1.0 =
Major update with enhanced theme integration, authentic brand logos, and improved user experience. All buttons are now enabled by default.

= 1.0.0 =
Initial release of AI Share Buttons plugin.
