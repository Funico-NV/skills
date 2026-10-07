# Abstract Operational Dashboard Example

This example demonstrates the preferred density and hierarchy without referencing any real codebase.

```swift
struct DashboardPage: View {

    var body: some View {
        PageShell {
            SiteHeader()

            Tabs {
                Tab("Optimum", isSelected: true)
                Tab("Batch analysis")
                Tab("Scenarios")
                Tab("Data")
            }

            Grid(columns: 4, spacing: 12) {
                MetricCard(label: "Material use", value: "86.7%")
                MetricCard(label: "Total remainder", value: "16,267 mm")
                MetricCard(label: "Valid patterns", value: "4")
                MetricCard(label: "Efficiency", value: "-")
            }

            Panel(title: "Optimal pattern mix") {
                DataTable {
                    Row("rail + shoulder", quantity: "20", remainder: "343 mm")
                    Row("rail + foot", quantity: "20", remainder: "417 mm")
                }
            }
        }
    }
}
```
