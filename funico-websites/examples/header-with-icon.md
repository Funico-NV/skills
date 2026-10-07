# Abstract Header With Icon Example

This example shows design intent only. It is not real Funico code and does not refer to a real framework.

```swift
struct SiteHeader: View {

    var body: some View {
        Header {
            HStack(spacing: 16) {

                SiteIcon(symbol: .precisionMark)
                    .tint(.base)
                    .supportTint(.secondary)
                    .frame(width: 52, height: 52)

                VStack(alignment: .leading, spacing: 4) {
                    Text("Website Name")
                        .font(.brandTitle)

                    Text("Production intelligence")
                        .font(.caption)
                        .foregroundStyle(.muted)
                }

                Spacer()

                Navigation {
                    Tab("Overview", isSelected: true)
                    Tab("Planning")
                    Tab("Data")
                }
            }
        }
    }
}
```
