# View ID

## View IDs in Land Explorer

OmicSoft Lands contain dozens of Views to allow users to explore all aspects of Land data. However, the sheer number of Views can be daunting to the new user.

Array Server admins can choose to hide a subset of Views from certain groups of users, such as new users.

Admins can customize the set of listed Views to only the most commonly used Views for each level of information.

## Basic Usage

  1. View ID: The name of the View to be selectively displayed
  2. ContextType: The Level of data, such as "Gene". If not provided, all matches to the View ID will be affected.
  3. Includes/Excludes:A list of groups or users that should or should not see this View
    Multiple users and user groups can be specified
      a. UserIDs can be listed directly, separated by commas
      b. UserGroups should be preceded by [usergroup]
  4. If a user's ID or any associated group is included, the user will be affected.
  5. In general, Excludes and Includes should not be specified at the same time. If both are specified, then
      -If user belongs to a group in "Excludes" list, it will be excluded directly without checking "Includes";
      -If user does not belong to a group in "Excludes" list, he/she can only have the view when the user belong to a group in "Includes" list.
    administrators are also filtered based on this rule.
