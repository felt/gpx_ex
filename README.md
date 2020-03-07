# GpxEx

Small Elixir library for parsing GPX files. GPX schema definition: https://www.topografix.com/GPX/1/1

## Installation

**NOT ON HEX YET.**

## Usage

```elixir
iex(1)> {:ok, gpx_doc} = File.read("./my_track.gpx")
iex(2)> GpxEx.parse(gpx_doc)

%GpxEx.Gpx{
  tracks: [
    %GpxEx.Track{
      segments: [
        %GpxEx.TrackSegment{
          points: [
            %GpxEx.TrackPoint{
              ele: 10.2,
              lat: 54.519848,
              lon: 18.539699,
              time: "2020-02-02T10:37:13Z"
            },
            %GpxEx.TrackPoint{
              ele: 10.2,
              lat: 54.519854,
              lon: 18.53973,
              time: "2020-02-02T10:37:14Z"
            }
          ]
        }
      ]
    }
  ]
}
```

## TODO

[] get track's name
