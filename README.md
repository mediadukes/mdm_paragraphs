# Custom Drupal 8 module for pre-configured paragraphs types

This module adds a few pre-configured paragraph types:

- Text (for basic body text fields)
- View (to reference views blocks using the [viewsreference](https://www.drupal.org/project/viewsreference) module)

Four optional paragraph types can be installed (independently) if each of their dependencies are met:

- Form (to reference [webforms](https://www.drupal.org/project/webform))
- Image (to reference media using the custom [mdm_media](https://github.com/mediadukes/mdm_media) module)
- Layout (to create multi column/row paragraphs)
- Block (to reference blocks using an [entity_browser](https://www.drupal.org/project/entity_browser) to select existing blocks)

More paragraph types will be added later.

## Usage

Just install as any other drupal module using `composer require`.

```
composer require mediadukes/mdm_paragraphs:^1.0
```

If it's not already present in your repositories array you'll need to define inside your root `composer.json` where mediadukes packages can be found.

```
"repositories": [
  {
    "type": "composer",
    "url": "https://packages.mediadukes.be"
  }
]
```

Or you can use the [mediadukes drupal-project template](https://github.com/mediadukes/drupal-project) where all of this is already added via the custom [Amatus profile](https://github.com/mediadukes/mdp_amatus).
