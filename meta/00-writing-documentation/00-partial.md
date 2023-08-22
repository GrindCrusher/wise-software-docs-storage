# Partial

Easily duplicate content without rewriting it.

# Motivation

In our documentation, it is sometimes needed to display the same content in multiple places. Simply copying and pasting it would make documentation harder to maintain.

Partials are a feature that solve this. You would keep the duplicated content in one place.

# Creating Partials

Partials are created in the `/partials` folder. You will have three places to put it:
- `common` includes Partials used in multiple environments;
- `enterprise` includes Partials used only in the Enterprise environment;
- `mobile` includes Partials used only in the Mobile environment.

You may add more folders, or even not use a folder at all. They are there for the sake of organization.

Add a file under the folder you'd like to place it in, and give it a name (ending in `.md`). Examples include `/billing.md`, `/mobile/navigation.md`, or `/mobile/work-orders/customers.md`.

## Writing Partial Content

There is no special syntax for Partials. It supports the same syntax as a regular documentation page. You would put the repeated information in the Partial file. To display: 

### Partial Example
This is an **example** of a Partial.

You would write the following in the partial file:
```md
### Partial Example
This is an **example** of a Partial.
```

# Using Partials

Use the Partial component: `@​partial[path]`. The path argument would be the path to the partial file, starting from the partials folder. For example, if your partial is in `/partials/common/example.md`, you would write `@​partial[/common/example.md]`.

Make sure that the partial is on its own line! It should look like this:
```md
Paragraph.

@​partial[/common/example.md]

Other paragraph.
```

# Seeing if the Partial Worked

If the partial worked, it would display on the website. If it doesn't, you'll see an error where it should be:

@partial:fail

The most likely cause of this error is that the path you typed in wasn't correct.

# Partial Spec

```md
@​partial[Path path]
@partial:fail
```
## Primary

```md
@​partial[Path path]
```

Embed a partial.

| Parameter | Type | Description                                         |
| --------- | ---- | --------------------------------------------------- |
| path      | Path | The path to the partial. Do not include `/partial`. |

## `fail` State

```md
@partial:fail
```

The state shown when a Partial fails to load. Could be used directly, but is not recommended.

This state does not accept any parameters.
