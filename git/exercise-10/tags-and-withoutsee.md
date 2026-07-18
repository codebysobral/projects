# Difference Between a Lightweight Tag and an Annotated Tag

- **Lightweight Tag** – A simple tag that points 
directly to a commit. It is commonly used to mark 
local versions or temporary milestones. It is 
created with:

  ```bash
  git tag <tag-name>
  ```

- **Annotated Tag** – A tag stored as a full Git 
object, containing additional metadata such as 
the tagger's name, email, date, and an optional 
message. It is typically used to mark official 
releases that will be shared with remote 
repositories. It is created with:

  ```bash
  git tag -a <tag-name> -m "<tag-message>"
  ```

## Example of Versioning

| Version Change | Type | Reason |
|----------------|------|--------|
| `v1.2.3` → `v1.2.4` | **PATCH** | Fixed a bug in the username field during login. |
| `v1.2.4` → `v1.3.0` | **MINOR** | Added a new feature to the login system. |
| `v1.3.0` → `v2.0.0` | **MAJOR** | Redesigned the login system, introducing breaking changes to improve security. |

