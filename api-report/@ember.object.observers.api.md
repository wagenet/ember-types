## API Report File for "@ember/object-observers"

> Do not edit this file. It is a report generated by [API Extractor](https://api-extractor.com/).

```ts

import { ObserverMethod } from '@ember/object/-private/types';

// @public
export function addObserver<Context, Target>(
obj: Context,
key: keyof Context,
target: Target,
method: ObserverMethod<Target, Context>
): void;

// @public (undocumented)
export function addObserver<Context>(
obj: Context,
key: keyof Context,
method: ObserverMethod<Context, Context>
): void;

// @public
export function removeObserver<Context, Target>(
obj: Context,
key: keyof Context,
target: Target,
method: ObserverMethod<Target, Context>
): any;

// @public (undocumented)
export function removeObserver<Context>(
obj: Context,
key: keyof Context,
method: ObserverMethod<Context, Context>
): any;

// (No @packageDocumentation comment for this package)

```
