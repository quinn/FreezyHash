FreezyHash
==========

a silly way to preserve a value of a hash. 

## Usage:

    hash = FreezyHash.new({a: 'hash'})
    hash.freezy(:a)
    hash[:a] = 'new value' #=> Warning: can't change key a
