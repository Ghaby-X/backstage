## API Report File for "@backstage/backend-defaults"

> Do not edit this file. It is a report generated by [API Extractor](https://api-extractor.com/).

```ts
import type { Config } from '@backstage/config';
import { ConfigSchema } from '@backstage/config-loader';
import { LoggerService } from '@backstage/backend-plugin-api';
import { RemoteConfigSourceOptions } from '@backstage/config-loader';
import { RootConfigService } from '@backstage/backend-plugin-api';
import { ServiceFactory } from '@backstage/backend-plugin-api';

// @public (undocumented)
export function createConfigSecretEnumerator(options: {
  logger: LoggerService;
  dir?: string;
  schema?: ConfigSchema;
}): Promise<(config: Config) => Iterable<string>>;

// @public
export interface RootConfigFactoryOptions {
  argv?: string[];
  remote?: Pick<RemoteConfigSourceOptions, 'reloadInterval'>;
  // (undocumented)
  watch?: boolean;
}

// @public (undocumented)
export const rootConfigServiceFactory: ((
  options?: RootConfigFactoryOptions,
) => ServiceFactory<RootConfigService, 'root', 'singleton'>) &
  ServiceFactory<RootConfigService, 'root', 'singleton'>;

// Warnings were encountered during analysis:
//
// src/entrypoints/rootConfig/createConfigSecretEnumerator.d.ts:5:1 - (ae-undocumented) Missing documentation for "createConfigSecretEnumerator".
// src/entrypoints/rootConfig/rootConfigServiceFactory.d.ts:20:5 - (ae-undocumented) Missing documentation for "watch".
// src/entrypoints/rootConfig/rootConfigServiceFactory.d.ts:26:22 - (ae-undocumented) Missing documentation for "rootConfigServiceFactory".

// (No @packageDocumentation comment for this package)
```