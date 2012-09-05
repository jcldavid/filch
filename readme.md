# Filch Laravel Bundle

Extend the file cache functionality of Laravel to support (insert right word here).

## Installation

1. Add Filch to your bundles.php

		'filch' => ['auto' => true]

2. Use the `filch` as your cache driver in `configs/cache.php`

		'driver' => 'filch'

3. Or use it manually

		$cache = Cache::driver('filch');
		$cache->put('this', 'that', 454545);


## Usage

	Cache::put('latest.posts', $data, 343434);

Creates a directory `latest` and a file `posts`

	Cache::purge('latest');

Empties the `latest` directory

## Credits

To each and every one of you. Mwah!