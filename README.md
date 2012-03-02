# [balance3D](indamix.github.com/balance3D)

## Start balancing element

`balance3D(element[, options]);`

## Options

	options = {
		perspective: pixels,
		/*
			Distance in pixels.
			You can think of it as though you’re looking at the page from a such distance away.
			Default: 1000
		*/
		smooth: seconds
		/*
			Orientation information from device gets jitter, smoothing will improve visual perception
			Time in seconds to smooth the animation
			Default: .3
		*/
	}

### Examples

	balance3D(document.getElementById('elm'))

	balance3D(document.getElementById('elm'), { perspective: 500 })

	balance3D(document.getElementById('elm'), { smooth: 1 })

	balance3D(document.getElementById('elm'), { perspective: 300, smooth: .2 })

## Stop balancing element(s)

Stop balancing element _elm_
	balance3D.stop(elm)

Stop balancing all elements
	balance3D.stop()