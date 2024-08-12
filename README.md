1. npm install
2. npx tsc

### typescript 5.5.4:
no errors

### typescript 5.6.0-beta:

```
node_modules/lru-cache/dist/commonjs/index.d.ts:973:5 - error TS2416: Property 'entries' in type 'LRUCache<K, V, FC>' is not assignable to the same property in base type 'Map<K, V>'.
  Type '() => Generator<[K, V], void, unknown>' is not assignable to type '() => BuiltinIterator<[K, V], undefined, any>'.
    Call signature return types 'Generator<[K, V], void, unknown>' and 'BuiltinIterator<[K, V], undefined, any>' are incompatible.
      The types returned by 'next(...)' are incompatible between these types.
        Type 'IteratorResult<[K, V], void>' is not assignable to type 'IteratorResult<[K, V], undefined>'.
          Type 'IteratorReturnResult<void>' is not assignable to type 'IteratorResult<[K, V], undefined>'.
            Type 'IteratorReturnResult<void>' is not assignable to type 'IteratorReturnResult<undefined>'.
              Type 'void' is not assignable to type 'undefined'.

973     entries(): Generator<[K, V], void, unknown>;
        ~~~~~~~

node_modules/lru-cache/dist/commonjs/index.d.ts:985:5 - error TS2416: Property 'keys' in type 'LRUCache<K, V, FC>' is not assignable to the same property in base type 'Map<K, V>'.
  Type '() => Generator<K, void, unknown>' is not assignable to type '() => BuiltinIterator<K, undefined, any>'.
    Call signature return types 'Generator<K, void, unknown>' and 'BuiltinIterator<K, undefined, any>' are incompatible.
      The types returned by 'next(...)' are incompatible between these types.
        Type 'IteratorResult<K, void>' is not assignable to type 'IteratorResult<K, undefined>'.
          Type 'IteratorReturnResult<void>' is not assignable to type 'IteratorResult<K, undefined>'.
            Type 'IteratorReturnResult<void>' is not assignable to type 'IteratorReturnResult<undefined>'.
              Type 'void' is not assignable to type 'undefined'.

985     keys(): Generator<K, void, unknown>;
        ~~~~

node_modules/lru-cache/dist/commonjs/index.d.ts:997:5 - error TS2416: Property 'values' in type 'LRUCache<K, V, FC>' is not assignable to the same property in base type 'Map<K, V>'.
  Type '() => Generator<V, void, unknown>' is not assignable to type '() => BuiltinIterator<V, undefined, any>'.
    Call signature return types 'Generator<V, void, unknown>' and 'BuiltinIterator<V, undefined, any>' are incompatible.
      The types returned by 'next(...)' are incompatible between these types.
        Type 'IteratorResult<V, void>' is not assignable to type 'IteratorResult<V, undefined>'.
          Type 'IteratorReturnResult<void>' is not assignable to type 'IteratorResult<V, undefined>'.
            Type 'IteratorReturnResult<void>' is not assignable to type 'IteratorReturnResult<undefined>'.
              Type 'void' is not assignable to type 'undefined'.

997     values(): Generator<V, void, unknown>;
        ~~~~~~

node_modules/lru-cache/dist/commonjs/index.d.ts:1009:5 - error TS2416: Property '[Symbol.iterator]' in type 'LRUCache<K, V, FC>' is not assignable to the same property in base type 'Map<K, V>'.
  Type '() => Generator<[K, V], void, unknown>' is not assignable to type '() => BuiltinIterator<[K, V], undefined, any>'.
    Call signature return types 'Generator<[K, V], void, unknown>' and 'BuiltinIterator<[K, V], undefined, any>' are incompatible.
      The types returned by 'next(...)' are incompatible between these types.
        Type 'IteratorResult<[K, V], void>' is not assignable to type 'IteratorResult<[K, V], undefined>'.
          Type 'IteratorReturnResult<void>' is not assignable to type 'IteratorResult<[K, V], undefined>'.
            Type 'IteratorReturnResult<void>' is not assignable to type 'IteratorReturnResult<undefined>'.
              Type 'void' is not assignable to type 'undefined'.

1009     [Symbol.iterator](): Generator<[K, V], void, unknown>;
         ~~~~~~~~~~~~~~~~~

node_modules/lru-cache/dist/commonjs/index.d.ts:1032:5 - error TS2416: Property 'forEach' in type 'LRUCache<K, V, FC>' is not assignable to the same property in base type 'Map<K, V>'.
  Type '(fn: (v: V, k: K, self: LRUCache<K, V, FC>) => any, thisp?: any) => void' is not assignable to type '(callbackfn: (value: V, key: K, map: Map<K, V>) => void, thisArg?: any) => void'.
    Types of parameters 'fn' and 'callbackfn' are incompatible.
      Types of parameters 'map' and 'self' are incompatible.
        Type 'LRUCache<K, V, FC>' is not assignable to type 'Map<K, V>'.
          The types returned by 'entries().next(...)' are incompatible between these types.
            Type 'IteratorResult<[K, V], void>' is not assignable to type 'IteratorResult<[K, V], undefined>'.
              Type 'IteratorReturnResult<void>' is not assignable to type 'IteratorResult<[K, V], undefined>'.
                Type 'IteratorReturnResult<void>' is not assignable to type 'IteratorReturnResult<undefined>'.
                  Type 'void' is not assignable to type 'undefined'.

1032     forEach(fn: (v: V, k: K, self: LRUCache<K, V, FC>) => any, thisp?: any): void;
         ~~~~~~~


Found 5 errors in the same file, starting at: node_modules/lru-cache/dist/commonjs/index.d.ts:973
```
