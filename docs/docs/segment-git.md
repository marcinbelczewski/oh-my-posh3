---
id: git
title: Git
sidebar_label: Git
---

## What

Display `git status` information when in a git repository. Also works for subfolders.
Local changes can also shown by default using the following syntax for both the working and staging area:

- `+` added
- `~` modified
- `-` deleted
- `?` untracked

## Sample Configuration

```json
{
  "type": "git",
  "style": "powerline",
  "powerline_symbol": "\uE0B0",
  "foreground": "#193549",
  "background": "#ffeb3b",
  "properties": {
    "display_stash_count": true,
    "display_upstream_icon": true
  }
}
```

## Properties

### Standard

- branch_icon: `string` - the icon to use in front of the git branch name - defaults to `\uE0A0 `
- branch_identical_icon: `string` - the icon to display when remote and local are identical - defaults to `\uF0C9`
- branch_ahead_icon: `string` - the icon to display when the local branch is ahead of its remote - defaults to `\uF176`
- branch_behind_icon: `string` - the icon to display when the local branch is behind its remote - defaults to `\uF175`
- branch_gone_icon: `string` - the icon to display when there's no remote branch - defaults to `\u2262`

### Status

- display_status: `boolean` - display the local changes or not - defaults to `true`
- display_status_detail: `boolean` - display the local changes in detail or not - defaults to `true`
- display_stash_count: `boolean` show stash count or not - defaults to `false`
- status_separator_icon: `string` icon/text to display between staging and working area changes - defaults to ` |`
- local_working_icon: `string` - the icon to display in front of the working area changes - defaults to `\uF044`
- local_staged_icon: `string` - the icon to display in front of the staged area changes - defaults to `\uF046`
- stash_count_icon: `string` icon/text to display before the stash context - defaults to `\uF692`

### HEAD context

- commit_icon: `string` - icon/text to display before the commit context (detached HEAD) - defaults to `\uF417`
- tag_icon: `string` - icon/text to display before the tag context - defaults to `\uF412`
- rebase_icon: `string` - icon/text to display before the context when in a rebase - defaults to `\uE728 `
- cherry_pick_icon: `string` - icon/text to display before the context when doing a cherry-pick - defaults to `\uE29B `
- merge_icon: `string` icon/text to display before the merge context - defaults to `\uE727 `
- no_commits_icon: `string` icon/text to display when there are no commits in the repo - defaults to `\uF594 `

### Upstream context

- display_upstream_icon: `boolean` - display upstream icon or not - defaults to `false`
- github_icon: `string` - icon/text to display when the upstream is Github - defaults to `\uF408 `
- gitlab_icon: `string` - icon/text to display when the upstream is Gitlab - defaults to `\uF296 `
- bitbucket_icon: `string` - icon/text to display when the upstream is Bitbucket - defaults to `\uF171 `
- azdo_icon: `string` - icon/text to display when the upstream is Azure DevOps - defaults to `\uE70C `
- git_icon: `string` - icon/text to display when the upstream is not known/mapped - defaults to `\uE5FB `

### Colors

- working_color: `string` [color][colors] - foreground color for the working area status - defaults to segment foreground
- staging_color: `string` [color][colors] - foreground color for the staging area status - defaults to segment foreground
- status_colors_enabled: `boolean` - color the segment based on the repository status - defaults to `false`
- color_background: `boolean` - color background or foreground - defaults to `true`
- local_changes_color: `string` [color][colors] - segment color when there are local changes - defaults to segment
foreground/background (see `color_background`)
- ahead_and_behind_color: `string` [color][colors] - segment color when the branch is ahead and behind -
defaults to segment foreground/background (see `color_background`)
- behind_color: `string` [color][colors] - segment color when the branch is behind - defaults to segment
foreground/background (see `color_background`)
- ahead_color: `string` [color][colors] - segment color when the branch is ahead - defaults to segment
foreground/background (see `color_background`)

[colors]: /docs/configure#colors
