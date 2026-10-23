# Abstract Header With Icon Example

This example shows design intent only. It is not real Funico code and does not refer to a real framework. Match the [current reference](../assets/design-reference.png): a compact white menu bar with inline navigation and a small, clearly rendered icon.

```swift
struct SiteHeader: View {

    var body: some View {
        Header {
            HStack(spacing: 28) {

                HStack(spacing: 10) {
                    SiteIcon(symbol: .precisionMark)
                        .tint(.base)
                        .supportTint(.secondary)
                        .frame(width: 32, height: 32)

                    Text("Website Name")
                        .font(.brandTitleCompact)
                }
                .fixedSize()

                PrimaryNavigation {
                    NavigationLink("Overview", isCurrentPage: true)
                    NavigationLink("Planning")
                    NavigationLink("Data")
                }
                .selectionStyle(.bottomUnderline(tint: .base, thickness: 2))

                Spacer()

                Text("Local workspace · 1.0")
                    .font(.caption)
                    .foregroundStyle(.muted)
            }
            .frame(minHeight: 58)
            .padding(.horizontal, 32)
        }
        .background(.white)
        .border(.bottom, color: .border)
    }
}
```

At narrow widths, move navigation into a compact menu or a scrollable row below the brand. Move or hide nonessential utility text before reducing brand space. Preserve comfortable hit areas and visible keyboard focus.
