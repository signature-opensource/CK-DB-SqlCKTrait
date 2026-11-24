Persists the `CKTrait` of CK.Core in the database: trait contexts, traits and their atomic words, with functions that
find the sub sets and super sets of a trait.

`CKTraitContextTable.RegisterContextAsync` registers a `CKTraitContext` and returns a `DBCKTraitContext`, whose
`DBCKTraitContext.FindOrCreateAsync` and `DBCKTraitContext.FindOnlyAsync` give a `DBCKTrait` (the trait and its
identifier). `CKTraitTable` finds, creates and destroys the traits; the `CK.fCKTraitSubSet`, `CK.fCKTraitSuperSet`,
`CK.fCKTraitProperSubSet` and `CK.fCKTraitProperSuperSet` functions compare them.
