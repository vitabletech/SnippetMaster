# Release Notes - All-in-One Snippet Master Extension (Version 1.2.1)

## What's Changed
- Release v1.2.0 by @pankajcs033 in Pull Request #28
- Full Changelog: [v1.2.0...v1.2.1](https://github.com/snippetmaster/snippets/compare/v1.2.0...v1.2.1)

### New Features
- Added new snippets for customizing the WordPress admin interface.
- Implemented functionality to hide and show custom menu items from the sidebar.
- Enabled the ability for ninjas to access and interact with other user roles without requiring a third-party plugin.
- Introduced new videos demonstrating how to contribute to Snippet Master.
- Included guidelines on how to release packages in Snippet Master.
- Expanded support for multiple languages.

### Bug Fixes
- Resolved the documentation table content issue.

### Improvements
- Updated documentation to reflect the latest changes and improvements.
- Implemented UI-related changes for a more intuitive user experience.

## Wordpress Snippets

| Prefix                                | Description                                                                                       |
|---------------------------------------|---------------------------------------------------------------------------------------------------|
| _hide_meta_boxes                      | Hide specific meta boxes for non-administrator users.                                            |
| _change_admin_menu_name               | Rename the Dashboard menu name.                                                                  |
| _remove_custom_column                 | Remove specific columns from a table. Replace 'column_key' with the key of the column you want to remove. |
| _unset_default_dashboard_widgets      | Unset all default widgets from the dashboard.                                                   |
| _custom_remove_admin_footer           | Remove version information from admin footer and display custom text.                           |
| _custom_remove_admin_bar_comments     | Remove comments from the admin bar.                                                             |
| _hide_admin_bar                       | Hide the admin bar.                                                                             |
| _custom_admin_footer_text             | Add custom footer text to the admin area.                                                       |
| _remove_wordpress_version_footer      | Remove the update footer or default WordPress version from the admin area.                     |
| _remove_screen_options                | Show screen options based on user capability. It means by super admin current_user_can('manage_options'). |
| _hide_screen_options                  | Hide screen options for all users except super admin.                                           |
| _change_admin_bar_title               | Change the welcome title in the top bar of the admin area from 'Howdy' to 'Hello'.              |
| _remove_new_button_admin              | Remove the '+ New' button from the top bar in the admin site.                                   |
| _remove_wordpress_logo                | Remove the WordPress logo from the admin bar.                                                   |
| _restrict_user_access                 | Restrict user access to specific pages based on their role.                                      |
| _custom_restrict_admin_menus          | Restrict specific admin menus for non-admin users.                                              |
| _custom_ninja_forms_submissions_permissions | Customize permissions for Ninja Forms submissions based on user capabilities.            |
| _custom_ninja_forms_all_permissions   | Customize permissions for Ninja Forms admin menus and API actions based on user capabilities.  |

## Contributors
- [@msrajawat298](https://github.com/msrajawat298)
- [@pankajcs033](https://github.com/pankajcs033)

## Installation
- Download the latest release from the [Releases](https://github.com/snippetmaster/snippets/releases) page.
- Extract the downloaded ZIP file to your plugins directory.
- Activate the "Snippet Master" plugin from the WordPress admin dashboard.

## Getting Started
- Refer to the documentation for detailed instructions on using the shell snippets: [Snippet Master Docs](https://snippetmaster.com/docs).

## Support and Feedback
- For any issues or questions, please open a new [issue](https://github.com/snippetmaster/snippets/issues).
- We welcome your feedback and contributions! See the guidelines for [contributing](https://github.com/snippetmaster/snippets/blob/main/CONTRIBUTING.md).