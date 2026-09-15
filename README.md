# How to bind the ListView data using RESTful API service in .NET MAUI SfListView?

This demo explains about how to bind the ListView data using RESTful API service in .NET MAUI SfListView?

## Sample

```xaml
<syncfusion:SfListView
                x:Name="listView"
                AutoFitMode="Height"
                ItemSpacing="5"
                ItemsSource="{Binding UserInfo}">
    <syncfusion:SfListView.ItemTemplate>
        <DataTemplate>
            <Border
                Margin="10,5"
                Padding="15"
                BackgroundColor="White"
                Stroke="#DDDDDD"
                StrokeShape="RoundRectangle 12"
                StrokeThickness="1">
                <Grid RowSpacing="8">
                    <Grid.RowDefinitions>
                        <RowDefinition Height="Auto" />
                        <RowDefinition Height="Auto" />
                        <RowDefinition Height="Auto" />
                        <RowDefinition Height="Auto" />
                    </Grid.RowDefinitions>

                    <Label
                        Grid.Row="0"
                        FontAttributes="Bold"
                        FontSize="16"
                        Text="Username:"
                        TextColor="#333" />
                    <Label
                        Grid.Row="0"
                        Grid.Column="1"
                        Margin="100,0,0,0"
                        FontSize="16"
                        HorizontalOptions="Start"
                        Text="{Binding [username]}"
                        TextColor="#555" />

                    <Label
                        Grid.Row="1"
                        FontAttributes="Bold"
                        FontSize="16"
                        Text="Website:"
                        TextColor="#333" />
                    <Label
                        Grid.Row="1"
                        Grid.Column="1"
                        Margin="100,0,0,0"
                        FontSize="16"
                        HorizontalOptions="Start"
                        Text="{Binding [website]}"
                        TextColor="#555" />

                    <Label
                        Grid.Row="2"
                        FontAttributes="Bold"
                        FontSize="16"
                        Text="Phone:"
                        TextColor="#333" />
                    <Label
                        Grid.Row="2"
                        Grid.Column="1"
                        Margin="100,0,0,0"
                        FontSize="16"
                        HorizontalOptions="Start"
                        Text="{Binding [phone]}"
                        TextColor="#555" />

                    <Label
                        Grid.Row="3"
                        FontAttributes="Bold"
                        FontSize="16"
                        Text="Email:"
                        TextColor="#333" />
                    <Label
                        Grid.Row="3"
                        Grid.Column="1"
                        Margin="100,0,0,0"
                        FontSize="16"
                        HorizontalOptions="Start"
                        Text="{Binding [email]}"
                        TextColor="#555" />
                </Grid>
            </Border>
        </DataTemplate>
    </syncfusion:SfListView.ItemTemplate>
</syncfusion:SfListView>
```

## Requirements to run the demo

* [Visual Studio 2017](https://visualstudio.microsoft.com/downloads/) or [Visual Studio for Mac](https://visualstudio.microsoft.com/vs/mac/)
* Xamarin add-ons for Visual Studio (available via the Visual Studio installer).

## Troubleshooting

### Path too long exception

If you are facing path too long exception when building this example project, close Visual Studio and rename the repository to short and build the project.
