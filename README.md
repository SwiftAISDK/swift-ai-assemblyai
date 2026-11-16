<!-- Generated distribution; edit the canonical repository. -->
# swift-ai-assemblyai 1.2.0

Independent Swift-native port of Vercel AI SDK. Source and upstream dispositions are in PROVENANCE.json and Porting/.

## Distribution manifest

Add this package to your SwiftPM dependencies:

```swift
.package(url: "https://github.com/SwiftAISDK/swift-ai-assemblyai.git", from: "1.2.0")
```

Products: `SwiftAIAssemblyAI`.
Contribute and report issues in the canonical SwiftAISDK repository.

## Authored usage guide

# AssemblyAI for Swift

`SwiftAIAssemblyAI` adds AssemblyAI to [SwiftAISDK](https://github.com/SwiftAISDK/SwiftAISDK), an independent Swift port of the Vercel AI SDK. It ports `@ai-sdk/assemblyai` and supports transcription.

Provider guide with models, options, streaming and errors:

- [AssemblyAI](https://swiftaisdk.github.io/SwiftAISDK/providers/assemblyai/)

## Usage

Add the `SwiftAI` product from `swift-ai-core` and the `SwiftAIAssemblyAI` product from this package to your target, then create the provider:

```swift
import SwiftAI
import SwiftAIAssemblyAI

let provider = try AIProviders.assemblyAI(configuration: AssemblyAIProviderSettings())
```

By default the provider reads `ASSEMBLYAI_API_KEY` from the environment; values set in `AssemblyAIProviderSettings` take precedence.

To use every provider through one dependency, add the complete [SwiftAISDK](https://github.com/SwiftAISDK/SwiftAISDK) package instead; see [Install](https://swiftaisdk.github.io/SwiftAISDK/getting-started/install/).

## Contributing

This package is exported from `Packages/swift-ai-assemblyai` in the canonical [SwiftAISDK](https://github.com/SwiftAISDK/SwiftAISDK) repository. Open issues and pull requests there.
