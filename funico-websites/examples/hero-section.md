# Abstract Hero Section Example

This example shows the permitted style for examples: declarative, Swift-like, and abstract. It must not be treated as real project API.

```swift
struct HeroSection: View {

    var body: some View {
        Section {
            VStack(alignment: .leading, spacing: 24) {

                Text("Software built around your workflow.")
                    .font(.display)

                Text(
                    "Custom applications, dashboards and internal tools with a calm operational interface."
                )
                .font(.bodyLarge)

                Button("Discover the system")
                    .buttonStyle(.primary)
            }
        }
    }
}
```
