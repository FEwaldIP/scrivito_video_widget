# scrivito_video_widget

[![Gem Version](https://badge.fury.io/rb/scrivito_video_widget.svg)](http://badge.fury.io/rb/scrivito_video_widget)
[![Code Climate](https://codeclimate.com/github/Scrivito/scrivito_video_widget/badges/gpa.svg)](https://codeclimate.com/github/Scirvito/scrivito_video_widget)

A Widget for Scrivito to add a video widget using projekktor.

## Installation

Add this lines to your application's `Gemfile`:

    gem 'scrivito_video_widget'

Add this line to your application Stylesheet manifest:

    *= require scrivito_video_widget

Add this line to your application javascript manifest:

    /= require scrivito_video_widget

Add a Filter to your content_browser

    scrivito.content_browser.filters = {
      obj_class: {
        field: '_obj_class',
        options: {
          Quote: {
            title: 'Video',
            icon: 'video',
            query: scrivito.obj_where('_obj_class', 'equals', 'Video'),
            preset: {
              _obj_class: 'Video'
            }
          }
        }
      }
    };
If you want to implement a Contextual filter, visit our [Documentation](https://scrivito.com/content-browser)!

## Changelog

See [Changelog](https://github.com/Scrivito/scrivito_video_widget/blob/master/CHANGELOG.md) for more
details.

## Contributing

1. Fork it ( https://github.com/Scrivito/scrivito_video_widget/fork )
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new Pull Request