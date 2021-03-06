## API Report File for "@backstage/backend-test-utils"

> Do not edit this file. It is a report generated by [API Extractor](https://api-extractor.com/).

```ts
import { Knex } from 'knex';

// Warning: (ae-missing-release-tag) "isDockerDisabledForTests" is exported by the package, but it is missing a release tag (@alpha, @beta, @public, or @internal)
//
// @public (undocumented)
export function isDockerDisabledForTests(): boolean;

// Warning: (ae-missing-release-tag) "TestDatabaseId" is exported by the package, but it is missing a release tag (@alpha, @beta, @public, or @internal)
//
// @public
export type TestDatabaseId =
  | 'POSTGRES_13'
  | 'POSTGRES_9'
  | 'MYSQL_8'
  | 'SQLITE_3';

// Warning: (ae-missing-release-tag) "TestDatabases" is exported by the package, but it is missing a release tag (@alpha, @beta, @public, or @internal)
//
// @public
export class TestDatabases {
  static create(options?: {
    ids?: TestDatabaseId[];
    disableDocker?: boolean;
  }): TestDatabases;
  // (undocumented)
  eachSupportedId(): [TestDatabaseId][];
  // Warning: (tsdoc-param-tag-missing-hyphen) The @param block should be followed by a parameter name and then a hyphen
  init(id: TestDatabaseId): Promise<Knex>;
  // (undocumented)
  supports(id: TestDatabaseId): boolean;
}

// (No @packageDocumentation comment for this package)
```
