# Mastodon Tweaks (Custom Bird UI Variants)

Custom server CSS variants based on Mastodon Bird UI v4.0.0.

This repository contains two maintained custom stylesheets:

- `mastodon_server_toot_posting.css`
- `mastodon_server_appearance_lgbt.css`

Both are now rebased to Mastodon Bird UI v4.0.0 (dark base).

## What Is Included

### 1) `mastodon_server_toot_posting.css`

Base:
- Mastodon Bird UI v4.0.0 dark (`dist/mastodon-bird-ui.css`)

Custom overrides preserved:
- Hides advanced UI elephant mascot panel (`.drawer__inner__mastodon`)
- Custom publish text: `Toot! 🐘💨`

Backup created during migration:
- `mastodon_server_toot_posting.css.bak-3.0.0`

### 2) `mastodon_server_appearance_lgbt.css`

Base:
- Mastodon Bird UI v4.0.0 dark (`dist/mastodon-bird-ui.css`)

Custom overrides preserved:
- Custom publish text: `Toot!`

Backup created during migration:
- `mastodon_server_appearance_lgbt.css.bak-1.5.7rc1`

## Why The New Files Are Smaller

The previous files contained duplicated legacy theme blocks. During migration, each file was rebuilt from a single clean 4.0.0 base and custom overrides were re-applied at the end.

## Install On Mastodon Server

1. In Mastodon Admin, open Appearance settings:
- `https://<your-instance>/admin/settings/appearance`

2. Choose the variant you want from this repo.

3. Copy the full CSS contents and paste into Custom CSS.

4. Save and hard refresh browser cache.

## Suggested Variant Use

- Use `mastodon_server_toot_posting.css` if you want the elephant-fart publish label and hidden advanced UI elephant panel.
- Use `mastodon_server_appearance_lgbt.css` if you want the simpler `Toot!` publish label variant.

## Rollback

If needed, restore previous files from backups:

- `mastodon_server_toot_posting.css.bak-3.0.0`
- `mastodon_server_appearance_lgbt.css.bak-1.5.7rc1`

## Upstream Reference

Official upstream project:
- https://github.com/ronilaukkarinen/mastodon-bird-ui

For dark default styling, upstream recommends `dist/mastodon-bird-ui.css`.
