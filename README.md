Things to check:

rubin_templates/analyse_no_template_visits.ipynb
template_counts
x = metric_plot.data
fp_area = len(x_footprint[x_footprint>0]) * pix_area

Do I really understand masked arrays? what is the difference to this and:

rubin_templates/survey_coverage.ipynb:
        m = maf.MetricBundle.load(f)
        data = m.metric_values.data
        mask = m.metric_values.mask
        footprint_area[filt][n] = len(data[~mask]) * pix_area