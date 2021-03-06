## API Report File for "@ember/runloop"

> Do not edit this file. It is a report generated by [API Extractor](https://api-extractor.com/).

```ts

import { AnyFn } from 'ember/-private/type-utils';
import { EmberMethod } from 'ember/-private/type-utils';
import { EmberMethodParams } from 'ember/-private/type-utils';
import { EmberMethodReturn } from 'ember/-private/type-utils';
import { EmberRunTimer } from '@ember/runloop/types';

// @public
export function begin(): void;

// @public
export function bind<T, M extends EmberMethod<T>>(
target: T,
method: M,
...args: any[]
): (...args: any[]) => EmberMethodReturn<T, M>;

// @public
export function cancel(timer: EmberRunTimer): boolean;

// @public
export function debounce(
method: AnyFn,
wait: number,
immediate?: boolean
): EmberRunTimer;

// @public (undocumented)
export function debounce<Target, M extends EmberMethod<Target>>(
...args: [
target: Target,
method: M,
...args: EmberMethodParams<Target, M>,
wait: number,
immediate?: boolean
]
): EmberRunTimer;

// @public
export function end(): void;

// @public
export function join<M extends AnyFn>(method: M, ...args: Parameters<M>): ReturnType<M> | undefined;

// @public (undocumented)
export function join<T, M extends EmberMethod<T>>(
target: T,
method: M,
...args: EmberMethodParams<T, M>
): EmberMethodReturn<T, M> | undefined;

// @public
export function later(method: AnyFn, wait: number): EmberRunTimer;

// @public (undocumented)
export function later<T, M extends EmberMethod<T>>(
...args: [
target: T,
method: M,
...args: EmberMethodParams<T, M>,
wait: number,
]
): EmberRunTimer;

// @public
export function next<T, M extends EmberMethod<T>>(
target: T,
method: M,
...args: EmberMethodParams<T, M>
): EmberRunTimer;

// @public (undocumented)
export function next<M extends AnyFn>(
method: M,
...args: Parameters<M>
): EmberRunTimer;

// @public
export function once<T, M extends EmberMethod<T>>(
target: T,
method: M,
...args: EmberMethodParams<T, M>
): EmberRunTimer;

// @public
export function run<M extends AnyFn>(method: M): ReturnType<M>;

// @public (undocumented)
export function run<T, M extends EmberMethod<T>>(target: T, method: M, ...args: EmberMethodParams<T, M>): EmberMethodReturn<T, M>;

// @public
export function schedule<T, M extends EmberMethod<T>>(
queue: EmberRunQueues,
target: T,
method: M,
...args: EmberMethodParams<T, M>
): EmberRunTimer;

// @public (undocumented)
export function schedule<M extends AnyFn>(
queue: EmberRunQueues,
method: M,
...args: Parameters<M>
): EmberRunTimer;

// @public
export function scheduleOnce<T, M extends EmberMethod<T>>(
queue: EmberRunQueues,
target: T,
method: M,
...args: EmberMethodParams<T, M>
): EmberRunTimer;

// @public
export function throttle(
method: AnyFn,
spacing: number,
immediate?: boolean
): EmberRunTimer;

// @public (undocumented)
export function throttle<T, M extends EmberMethod<T>>(
...args: [
target: T,
method: M,
...methodArgs: EmberMethodParams<T, M>,
spacing: number,
immediate?: boolean
]
): EmberRunTimer;

// (No @packageDocumentation comment for this package)

```
