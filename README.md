# NAME

MojoX::JSON::XS - A JSON::XS backend replacement for Mojo::JSON

# SYNOPSIS

    sub startup
    {
        # ...

        $self->plugin('MojoX::JSON::XS');

        # ...
    }
    

# DESCRIPTION

Replaces Mojo::JSON methods encode, deocde and j with JSON::XS equivalient.
This gives faster processing, and removes the unnecessary encode of '/' chars in strings.

# FEATURES

It does not gracefully handle or skip blessed hashes
