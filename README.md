git-test-repository
===================

This repository contains all the "special cases" of objects that I
know of.

The (Perl) program used to build it can be found at:
http://github.com/book/git-test-repo-tool/

The test repository itself is entirely regenerated whenever I update the
builder script. If you use it in your tests, you should generate a bundle
with the `build-test-repo` program found in the `git-test-repo-tool`
repository and use that.

Here's an ascii-art view of the annotated commit graph,
with the details related to each commit:

    *   2547b1f6e678767d8b99dcf7de0bce7af3fcc742 (HEAD, master) iso-8859-1 message, gpgsig, mergetag
    |\  
    | * ddb3af4f0dbb790d2b3bf4c0dcb01bc1ccfb1d09 (tag: v1.0.3, encoding) commit with empty message
    * |   f57d3de36bcf54876203a90bed6e34c66445955a mergetag, gpgsig
    |\ \  
    | |/  
    * |   26ec45feb9a4fec8e5f5b9df3c8c74cd0c02ec35 iso-8859-1 message, mergetag
    |\ \  
    | | | *-.   443ccf76e57860fc1c9a571d9352e83767f892ab (mergetags) mergetag, mergetag
    | | | |\ \  
    | |_|_|/ /  
    |/| | | /   
    | | |_|/    
    | |/| |     
    | | | | *-.   61bb82c2b6b2dc821d246da296a614980bda798a (slave) mergetag, mergetag, gpgsig
    | | | | |\ \  
    | |_|_|_|/ /  
    |/| | | | /   
    | | | |_|/    
    | | |/| |     
    | | * | | 6f5aa7f9e1e7bd62459c162fefada15cbc4a31aa (tag: v1.0.2) utf-8 content, iso-8859-1 message, gpgsig
    | |/ / /  
    | * | | 9e9de230f26400f80f950ea2100120b6ed0866ff (tag: v1.0.1) shift-jis content, shift-jis message
    * | | |   046d7e6f44a34baa6f001c609ed9686ab99b541e (tag: v1.1.0) mergetag
    |\ \ \ \  
    | |/ / /  
    | * | | df54401d5437c692a7710ffcb13407231e59716f (tag: v1.0.0) utf-8 content, iso-8859-1 message and author name
    | * | | 14698909a83019a37cffa67307c95ce62702428e utf-8 content, iso-8859-1 message
    | |/ /  
    * | | 0f1bd12c68069a4bb737ae7e83f3560d0f0ba86c gpgsig
    * | | cdc334b5c3bfabb22beb95ba23546dd01b382b40 utf-8 content, utf-8 message
    |/ /  
    * |   1fcb030d541bc55c49c5594936dd88016b6a6744 basic merge
    |\ \  
    | |/  
    | * 9f5d6163102d412e67d166ae401346b0588e0229 empty tree, parentless
    * cd3ebcdff22498b4d78e55cd8b710afba41bff59 utf-8 author name, utf-8 message, utf-8 content
    * fc26f823bbc307264d42307f3fb14948a3ef1d53 no author name

Here's the list of the references in the repository,
with the details related to each of the annotated tags:

    ddb3af4f0dbb790d2b3bf4c0dcb01bc1ccfb1d09 refs/heads/encoding
    2547b1f6e678767d8b99dcf7de0bce7af3fcc742 refs/heads/master
    443ccf76e57860fc1c9a571d9352e83767f892ab refs/heads/mergetags
    61bb82c2b6b2dc821d246da296a614980bda798a refs/heads/slave
    ec70b772b61ac02366bfa415cbd0ae2def2853cd refs/tags/empty tag pointing to a tree (the empty tree)
    abc305df034369a366a4dcf46bb3ec18dd046449 refs/tags/hello tag pointing to a blob
    2754ad0190c4d6c7c9aab73782b6b83632d5a2cd refs/tags/v1.0.0 gpgsig
    a6f80fd17a885b5cef81be286a5615f2ea653ce0 refs/tags/v1.0.1 utf-8 message, gpgsig
    6400d8db7d50f3594d62e00f177cd849246a083e refs/tags/v1.0.2 gpgsig
    f98aa5d408b4153ce8b7528b832f46552f49de6c refs/tags/v1.0.3 gpgsig
    f63634769f7e15bca9404a9c019487290a3222f9 refs/tags/v1.1.0 gpgsig

