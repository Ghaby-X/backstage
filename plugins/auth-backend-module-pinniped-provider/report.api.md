## API Report File for "@backstage/plugin-auth-backend-module-pinniped-provider"

> Do not edit this file. It is a report generated by [API Extractor](https://api-extractor.com/).

```ts
import { BackendFeature } from '@backstage/backend-plugin-api';
import { BaseClient } from 'openid-client';
import { Config } from '@backstage/config';
import { OAuthAuthenticator } from '@backstage/plugin-auth-node';
import { Strategy } from 'openid-client';
import { TokenSet } from 'openid-client';

// @public @deprecated (undocumented)
export const authModulePinnipedProvider: BackendFeature;

// @public (undocumented)
const authModulePinnipedProvider_2: BackendFeature;
export default authModulePinnipedProvider_2;

// @public (undocumented)
export const pinnipedAuthenticator: OAuthAuthenticator<
  PinnipedStrategyCache,
  unknown
>;

// @public (undocumented)
export class PinnipedStrategyCache {
  constructor(callbackUrl: string, config: Config);
  // (undocumented)
  getStrategy(): Promise<{
    providerStrategy: Strategy<
      {
        tokenset: TokenSet;
      },
      BaseClient
    >;
    client: BaseClient;
  }>;
}

// Warnings were encountered during analysis:
//
// src/authenticator.d.ts:4:1 - (ae-undocumented) Missing documentation for "PinnipedStrategyCache".
// src/authenticator.d.ts:11:5 - (ae-undocumented) Missing documentation for "getStrategy".
// src/authenticator.d.ts:20:22 - (ae-undocumented) Missing documentation for "pinnipedAuthenticator".
// src/deprecated.d.ts:5:22 - (ae-undocumented) Missing documentation for "authModulePinnipedProvider".
// src/module.d.ts:2:22 - (ae-undocumented) Missing documentation for "authModulePinnipedProvider".
```