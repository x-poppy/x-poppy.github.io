# I18n Design

The default local is `en_US`. Below is the server side i18n key design.

## Naming Standard

Pascal Snake Case Naming. eg User_Name, App_Name

## Naming Strut Standard

AAA_BBB_CCC

AAA: the feature module name, if this feature is across many point it should be the `Common`.
BBB: the feature attribute name
CCC: the extension for the feature attribute, it optional. eg. Login_User_Name_Length_Validation

## Typesetting Standard

The Same feature module should in same typesetting block which new line on top and bottom.

```bash

AAA_XXX_001
AAA_XXX_002
AAA_XXX_003

BBB_XXX_001
BBB_XXX_002
BBB_XXX_003

```

## Comments Standard

We should add the comments(feature module name) for the block of i18n keys. If the the message of i18n is a template message, we should explain the parameter for the template message


```bash
# login
# parameter {0} means the min length of User_Name, {1} means the max length of User_Name
Login_User_Name_Length_Validation=User Name should more than {0} characters and less than {1} characters
```

## I18n Key List

```bash
# common

# login
# parameter {0} means the min length of User_Name, {1} means the max length of User_Name
Login_User_Name_Length_Validation=User Name should more than {0} characters and less than {1} characters
# parameter {0} means the min length of User_Password, {1} means the max length of User_Password
Login_User_Password_Length_Validation=User Password should more than {0} characters and less than {1} characters
```